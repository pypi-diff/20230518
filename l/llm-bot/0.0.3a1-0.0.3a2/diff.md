# Comparing `tmp/llm_bot-0.0.3a1.tar.gz` & `tmp/llm_bot-0.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bot-0.0.3a1.tar", max compression
+gzip compressed data, was "llm_bot-0.0.3a2.tar", max compression
```

## Comparing `llm_bot-0.0.3a1.tar` & `llm_bot-0.0.3a2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.3a1/LICENSE
--rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.3a1/README.md
--rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.3a1/llm_bot/__init__.py
--rw-r--r--   0        0        0    18008 2023-05-15 21:26:35.731820 llm_bot-0.0.3a1/llm_bot/core.py
--rw-r--r--   0        0        0      942 2023-05-15 21:34:38.581478 llm_bot-0.0.3a1/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.3a1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.3a2/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.3a2/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.3a2/llm_bot/__init__.py
+-rw-r--r--   0        0        0    18603 2023-05-18 17:31:17.612380 llm_bot-0.0.3a2/llm_bot/core.py
+-rw-r--r--   0        0        0      942 2023-05-18 17:32:08.332217 llm_bot-0.0.3a2/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.3a2/PKG-INFO
```

### Comparing `llm_bot-0.0.3a1/LICENSE` & `llm_bot-0.0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bot-0.0.3a1/llm_bot/core.py` & `llm_bot-0.0.3a2/llm_bot/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,127 +13,116 @@
 from langchain.schema import BaseMessage, HumanMessage, SystemMessage
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.vectorstores import FAISS
 import requests
 
 CONTEXT_INDEX_FILENAME = "index.faiss"
 CONTEXT_STORE_FILENAME = "store.pickle"
-CHAT_INDEX_FILENAME = "chat_index.faiss"
-CHAT_STORE_FILENAME = "chat_store.pickle"
 
 
 class BaseLLMBot(ABC):
     def __init__(
         self,
         text_chunk_size: int = 1000,
         text_chunk_overlap: int = 250,
         text_separators: List[str] = [" ", ".", ",", ";", ":", "!", "?", "\n"],
         temperature: float = 0,
     ):
-        self._store: FAISS = None
-        self._chat_store: FAISS = None
+        self._stores: Dict[str, FAISS] = None
         self._chat = ChatOpenAI(temperature=temperature)
         self._text_chunk_size = text_chunk_size
         self._text_chunk_overlap = text_chunk_overlap
         self._text_separators = text_separators
 
     @abstractmethod
-    def train(self, *args, **kwargs) -> None:
+    def train(self, name, *args, **kwargs) -> None:
         """
         Builds the index and the vector store from the given data.
         """
 
     @abstractmethod
-    def add_to_index(self, *args, **kwargs) -> None:
+    def add_to_index(self, name, *args, **kwargs) -> None:
         """
         Adds the given data to the index and the vector store.
         """
 
     def fetch_from_index(
-        self, query: str, n_results: int, index: str = "context", min_score: float = 0.0
+        self,
+        query: str,
+        n_results: int,
+        index: str,
+        min_score: float = 0.0,
     ) -> Tuple[List[Document], List[float]]:
         """
         Fetches the most relevant documents from the index.
 
         Args:
             query (str): The query to search for.
             n_results (int): The number of results to return.
-            index (str): The index to search in. Either 'context' or 'chat_history'.
+            index (str): The index to search in.
             min_score (float): The minimum score a document must have to be returned.
+            index_name (str): The name of the index to search in. If None, any index will be
+                searched.
 
         Returns:
             List[Document]: The most relevant documents.
         """
-        if index == "context":
-            docs_and_scores: List[
-                Tuple[Document, float]
-            ] = self._store.similarity_search_with_relevance_scores(query, k=n_results)
-            docs: List[Document] = [doc for doc, _ in docs_and_scores]
-            scores: List[float] = [score for _, score in docs_and_scores]
-        elif index == "chat_history":
-            if self._chat_store is None:
-                raise ValueError("No chat history available.")
-            docs_and_scores: List[
-                Tuple[Document, float]
-            ] = self._chat_store.similarity_search_with_relevance_scores(
-                query, k=n_results
-            )
-            docs: List[Document] = [doc for doc, _ in docs_and_scores]
-            scores: List[float] = [score for _, score in docs_and_scores]
-        else:
-            raise ValueError(f"Invalid index '{index}'.")
+        # Check if we have that index
+        if index not in self._stores:
+            raise ValueError(f"Index '{index}' does not exist.")
+        store = self._stores[index]
+        docs_and_scores: List[
+            Tuple[Document, float]
+        ] = store.similarity_search_with_relevance_scores(query, k=n_results)
+        docs: List[Document] = [doc for doc, _ in docs_and_scores]
+        scores: List[float] = [score for _, score in docs_and_scores]
         ret_docs: List[Document] = []
         ret_scores: List[float] = []
         for doc, score in zip(docs, scores):
             if score >= min_score:
                 ret_docs.append(doc)
                 ret_scores.append(score)
         return ret_docs, ret_scores
 
     def save(self, path: Union[str, Path]) -> None:
         """
-        Saves the index and the vector store to the given path.
+        Saves the indexes and the vector stores to the given path.
 
         Args:
             path (Union[str, Path]): The path to save the index and vector store to.
         """
         # Assert that the path exists
         path = Path(path)
         path.mkdir(parents=True, exist_ok=True)
 
-        # Save the indexes
-        index_fname = str(path / CONTEXT_INDEX_FILENAME)
-        faiss.write_index(self._store.index, index_fname)
-        if self._chat_store is not None:
-            chat_index_fname = str(path / CHAT_INDEX_FILENAME)
-            faiss.write_index(self._chat_store.index, chat_index_fname)
-
-        # Save the vector stores
-        index = self._store.index
-        self._store.index = None
-        store_fname = str(path / CONTEXT_STORE_FILENAME)
-        with open(store_fname, "wb") as f:
-            pickle.dump(self._store, f)
-        self._store.index = index
-        if self._chat_store is not None:
-            index = self._chat_store.index
-            self._chat_store.index = None
-            chat_store_fname = str(path / CHAT_STORE_FILENAME)
-            with open(chat_store_fname, "wb") as f:
-                pickle.dump(self._chat_store, f)
-            self._chat_store.index = index
+        # Save the indexes and the vector stores
+        indexes_list: List[str] = list(self._stores.keys())
+        for index_name in indexes_list:
+            # Get store and index from the index name
+            store = self._stores[index_name]
+            index = store.index
+            # Save index
+            index_fname = str(path / f"index_{index_name}.faiss")
+            faiss.write_index(index, index_fname)
+            # Save vector store
+            store.index = None
+            store_fname = str(path / f"store_{index_name}.pickle")
+            with open(store_fname, "wb") as f:
+                pickle.dump(store, f)
+            store.index = index
 
-    def download(self, url: str, path: Union[str, Path]) -> None:
+    def download(self, url: str, path: Union[str, Path], name: str) -> None:
         """
-        Downloads the model (index + vector store) from a given URL and extracts it to the given
+        Downloads the context (index + vector store) from a given URL and extracts it to the given
         path.
 
         Args:
-            url (str): The URL to download the model from.
-            path (Union[str, Path]): The path to extract the model to.
+            url (str): The URL to download the context from.
+            path (Union[str, Path]): The path to extract the context to.
+            name (str): The name of the context.
         """
         # Assert that the path exists
         path = Path(path)
         path.mkdir(parents=True, exist_ok=True)
 
         # Download the model
         response = requests.get(url, stream=True)
@@ -164,74 +153,79 @@
         except AssertionError as exc:
             index_fname.unlink(missing_ok=True)
             store_fname.unlink(missing_ok=True)
             raise AssertionError(
                 f"Either {index_fname} or {store_fname} does not exist."
             ) from exc
 
+        # If filenames are correct, rename them according to the context name
+        index_fname.rename(path / f"index_{name}.faiss")
+        store_fname.rename(path / f"store_{name}.pickle")
+
     def load(self, path: Union[str, Path]) -> None:
         """
         Loads the index and the vector store from the given path.
 
         Args:
             path (Union[str, Path]): The path to load the index and vector store from.
         """
         # Assert that the path exists
         path = Path(path)
         assert path.exists(), f"Path {path} does not exist."
 
-        # Assert that both files exist
-        index_fname = path / CONTEXT_INDEX_FILENAME
-        store_fname = path / CONTEXT_STORE_FILENAME
-        assert (
-            index_fname.exists() and store_fname.exists()
-        ), f"Either {index_fname} or {store_fname} does not exist."
-
-        # Load the index
-        index: IndexFlat = faiss.read_index(str(index_fname))
-
-        # Load the vector store
-        with open(store_fname, "rb") as f:
-            self._store: FAISS = pickle.load(f)
-        self._store.index = index
-
-        # Load chat stuff if it exists
-        chat_index_fname = path / CHAT_INDEX_FILENAME
-        chat_store_fname = path / CHAT_STORE_FILENAME
-        if chat_index_fname.exists() and chat_store_fname.exists():
-            chat_index: IndexFlat = faiss.read_index(str(chat_index_fname))
-            with open(chat_store_fname, "rb") as f:
-                self._chat_store: FAISS = pickle.load(f)
-            self._chat_store.index = chat_index
+        # Get list of files in the path with `index_` and `store_` prefixes
+        index_files = list(path.glob("index_*"))
+        store_files = list(path.glob("store_*"))
+
+        # Assert that all files have a corresponding index and store file
+        for index_file in index_files:
+            store_file = path / f"store_{index_file.name[6:]}.pickle"
+            assert store_file.exists(), f"Store file {store_file} does not exist."
+        for store_file in store_files:
+            index_file = path / f"index_{store_file.name[6:]}.faiss"
+            assert index_file.exists(), f"Index file {index_file} does not exist."
+
+        # Load the indexes and the vector stores
+        self._stores = {}
+        for index_file in index_files:
+            # Get index name from the index file name
+            index_name = index_file.name[6:]
+            # Load index
+            index: IndexFlat = faiss.read_index(str(index_file))
+            # Load vector store
+            store_fname = path / f"store_{index_name}.pickle"
+            with open(store_fname, "rb") as f:
+                store: FAISS = pickle.load(f)
+            store.index = index
+            self._stores[index_name] = store
 
     def build_messages(
         self,
         personality_prompt: str,
         user_message: str,
-        use_chat_history: bool = True,
+        use_chat_history: str = None,
         chat_history_prompt: str = "Aqui está o histórico da conversa até agora:",
         number_of_chat_history_docs: int = 2,
-        use_context: bool = True,
+        use_context: List[str] = None,
         context_prompt: str = "Aqui estão pedaços de informação que você pode usar:",
         number_of_context_docs: int = 2,
         minimum_similarity: float = 0.0,
     ) -> Tuple[List[BaseMessage], List[Tuple[str, float]]]:
         """
         Builds a list of messages to send to the chatbot.
 
         Args:
             personality_prompt (str): The prompt to use for the personality.
             user_message (str): The message from the user.
-            use_chat_history (bool, optional): Whether to use the chat history. Defaults to True.
+            use_chat_history (str, optional): Which chat history to use. Defaults to None.
             chat_history_prompt (str, optional): The prompt to use for the chat history. Defaults
                 to "Aqui está o histórico da conversa até agora:".
             number_of_chat_history_docs (int, optional): The number of chat history documents to
                 use. Defaults to 2.
-            use_context (bool, optional): Whether to search for context documents in the vector
-                store. Defaults to True.
+            use_context (List[str], optional): Which contexts to use. Defaults to None.
             context_prompt (str, optional): The prompt to use for the context documents. Defaults
                 to "Aqui estão pedaços de informação que você pode usar:".
             number_of_context_docs (int, optional): The number of context documents to use. Defaults
                 to 2.
             minimum_similarity (float, optional): The minimum similarity between the user message
                 and the context documents. Defaults to 0.0.
 
@@ -239,96 +233,104 @@
             Tuple[List[BaseMessage], List[str]]: A tuple containing the list of messages to send to
                 the chatbot and the list of sources of the context documents.
         """
         # Start list of messages with the personality prompt
         messages: List[BaseMessage] = [SystemMessage(content=personality_prompt)]
 
         # If we are using context, search for context documents and add them to the prompt
-        sources: List[str] = []
+        sources: List[Tuple[str, float]] = []
         if use_context:
             messages.append(SystemMessage(content=context_prompt))
-            docs, scores = self.fetch_from_index(
-                query=user_message,
-                n_results=number_of_context_docs,
-                index="context",
-                min_score=minimum_similarity,
-            )
-            # Store sources and their scores
-            sources = list(
-                set(
-                    [
-                        (str(doc.metadata["source"]), score)
-                        for doc, score in zip(docs, scores)
-                    ]
-                )
-            )
-            for doc in docs:
-                messages.append(SystemMessage(content=f"- {doc.page_content}"))
-
-        # If chat history is provided, add messages for it
-        if use_chat_history:
-            if self._chat_store:
-                messages.append(SystemMessage(content=chat_history_prompt))
-                docs, _ = self.fetch_from_index(
+            for context_name in use_context:
+                if len(sources) >= number_of_context_docs:
+                    break
+                docs, scores = self.fetch_from_index(
                     query=user_message,
-                    n_results=number_of_chat_history_docs,
-                    index="chat_history",
+                    n_results=number_of_context_docs,
+                    index=context_name,
+                    min_score=minimum_similarity,
+                )
+                # Store sources and their scores
+                tmp_sources = list(
+                    set(
+                        [
+                            (str(doc.metadata["source"]), score)
+                            for doc, score in zip(docs, scores)
+                        ]
+                    )
                 )
                 for doc in docs:
                     messages.append(SystemMessage(content=f"- {doc.page_content}"))
-                self._chat_store.add_texts(
+                for tmp_source in tmp_sources:
+                    sources.append(tmp_source)
+                    if len(sources) >= number_of_context_docs:
+                        break
+
+        # If chat history is provided, add messages for it
+        if use_chat_history:
+            messages.append(SystemMessage(content=chat_history_prompt))
+            docs, _ = self.fetch_from_index(
+                query=user_message,
+                n_results=number_of_chat_history_docs,
+                index=use_chat_history,
+            )
+            for doc in docs:
+                messages.append(SystemMessage(content=f"- {doc.page_content}"))
+            if use_chat_history in self._stores:
+                self._stores[use_chat_history].add_texts(
                     texts=[f"User: {user_message}"],
                     metadatas=[{"source": "user"}],
                 )
             else:
                 embedding = OpenAIEmbeddings()
-                self._chat_store = FAISS.from_texts(
+                self._stores[use_chat_history] = FAISS.from_texts(
                     texts=[f"User: {user_message}"],
                     embedding=embedding,
                     metadatas=[{"source": "user"}],
                 )
 
         # Add the user message
         messages.append(HumanMessage(content=user_message))
 
         return messages, sources
 
-    def chat(self, messages: List[BaseMessage]) -> str:
+    def chat(self, messages: List[BaseMessage], chat_id: str) -> str:
         """
         Sends the given messages to the chatbot and returns the response.
 
         Args:
             messages (List[BaseMessage]): The messages to send to the chatbot.
         """
         # Send the messages to the chatbot
         ai_message = self._chat(messages)
 
         # Get the response, add to index and return
         response = ai_message.content
-        if self._chat_store:
-            self._chat_store.add_texts(
+        if chat_id in self._stores:
+            self._stores[chat_id].add_texts(
                 texts=[f"Bot: {response}"],
                 metadatas=[{"source": "bot"}],
             )
         else:
             embedding = OpenAIEmbeddings()
-            self._chat_store = FAISS.from_texts(
+            self._stores[chat_id] = FAISS.from_texts(
                 texts=[f"Bot: {response}"],
                 embedding=embedding,
                 metadatas=[{"source": "bot"}],
             )
         return response
 
 
 class HTMLBot(BaseLLMBot):
-    def train(self, documents_path: Union[str, Path]) -> None:
+    def train(self, name: str, documents_path: Union[str, Path]) -> None:
         """
         Trains the bot using the given documents.
 
         Args:
+            name (str): The name of the knowledge base.
             documents_path (Union[str, Path]): The path to the documents to use for training.
             text_chunk_size (int, optional): The size of the text chunks to use for training.
                 Defaults to 1000.
             text_chunk_overlap (int, optional): The overlap between text chunks. Defaults to 250.
             text_separators (List[str], optional): The list of text separators to use for splitting
                 the text into chunks. Defaults to [" ", ".", ",", ";", ":", "!", "?", "\n"].
         """
@@ -350,21 +352,22 @@
         )
         docs: List[Document] = []
         for loader in loaders:
             docs.extend(loader.load_and_split(text_splitter=text_splitter))
 
         # Create the vector store
         embedding = OpenAIEmbeddings()
-        self._store = FAISS.from_documents(documents=docs, embedding=embedding)
+        self._stores[name] = FAISS.from_documents(documents=docs, embedding=embedding)
 
-    def add_to_index(self, html_files: List[Union[str, Path]]) -> None:
+    def add_to_index(self, name: str, html_files: List[Union[str, Path]]) -> None:
         """
         Adds the given HTML files to the index.
 
         Args:
+            name (str): The name of the knowledge base.
             html_files (List[Union[str, Path]]): The HTML files to add to the index.
         """
         # Import stuff (importing here avoids unnecessary dependencies)
         from langchain.document_loaders import BSHTMLLoader
 
         # Assert that all files exist
         html_files: List[Path] = [Path(html_file) for html_file in html_files]
@@ -381,27 +384,30 @@
             separators=self._text_separators,
         )
         docs: List[Document] = []
         for loader in loaders:
             docs.extend(loader.load_and_split(text_splitter=text_splitter))
 
         # Add the documents to the index
-        if self._store:
-            self._store.add_documents(documents=docs)
+        if name in self._stores:
+            self._stores[name].add_documents(documents=docs)
         else:
             embedding = OpenAIEmbeddings()
-            self._store = FAISS.from_documents(documents=docs, embedding=embedding)
+            self._stores[name] = FAISS.from_documents(
+                documents=docs, embedding=embedding
+            )
 
 
 class TextBot(BaseLLMBot):
-    def train(self, texts: List[str], metadatas: List[Dict[str, str]]):
+    def train(self, name: str, texts: List[str], metadatas: List[Dict[str, str]]):
         """
         Trains the bot using the given texts.
 
         Args:
+            name (str): The name of the knowledge base.
             texts (List[str]): The texts to use for training.
             metadatas (List[Dict[str, str]]): The metadata for each text.
         """
         # Assert that lengths match
         assert len(texts) == len(
             metadatas
         ), "Lengths of texts and metadatas do not match."
@@ -416,21 +422,24 @@
         for text, metadata in zip(texts, metadatas):
             docs_texts = text_splitter.split_text(text=text)
             for doc_text in docs_texts:
                 docs.append(Document(page_content=doc_text, metadata=metadata))
 
         # Create the vector store
         embedding = OpenAIEmbeddings()
-        self._store = FAISS.from_documents(documents=docs, embedding=embedding)
+        self._stores[name] = FAISS.from_documents(documents=docs, embedding=embedding)
 
-    def add_to_index(self, texts: List[str], metadatas: List[Dict[str, str]]):
+    def add_to_index(
+        self, name: str, texts: List[str], metadatas: List[Dict[str, str]]
+    ):
         """
         Adds the given texts to the index.
 
         Args:
+            name (str): The name of the knowledge base.
             texts (List[str]): The texts to add to the index.
             metadatas (List[Dict[str, str]]): The metadata for each text.
         """
         # Assert that lengths match
         assert len(texts) == len(
             metadatas
         ), "Lengths of texts and metadatas do not match."
@@ -444,12 +453,14 @@
         )
         for text, metadata in zip(texts, metadatas):
             docs_texts = text_splitter.split_text(text=text)
             for doc_text in docs_texts:
                 docs.append(Document(page_content=doc_text, metadata=metadata))
 
         # Add the documents to the index
-        if self._store:
-            self._store.add_documents(documents=docs)
+        if name in self._stores:
+            self._stores[name].add_documents(documents=docs)
         else:
             embedding = OpenAIEmbeddings()
-            self._store = FAISS.from_documents(documents=docs, embedding=embedding)
+            self._stores[name] = FAISS.from_documents(
+                documents=docs, embedding=embedding
+            )
```

### Comparing `llm_bot-0.0.3a1/pyproject.toml` & `llm_bot-0.0.3a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-bot"
-version = "0.0.3a1"
+version = "0.0.3a2"
 description = "Python library for developing LLM bots"
 authors = ["Gabriel Gazola Milan <gabriel.gazola@poli.ufrj.br>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/prefeitura-rio/chatbot-lab"
 repository = "https://github.com/prefeitura-rio/chatbot-lab"
 keywords = ["python", "chatbot", "bot", "llm"]
```

### Comparing `llm_bot-0.0.3a1/PKG-INFO` & `llm_bot-0.0.3a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-bot
-Version: 0.0.3a1
+Version: 0.0.3a2
 Summary: Python library for developing LLM bots
 Home-page: https://github.com/prefeitura-rio/chatbot-lab
 License: GPL-3.0-only
 Keywords: python,chatbot,bot,llm
 Author: Gabriel Gazola Milan
 Author-email: gabriel.gazola@poli.ufrj.br
 Requires-Python: >=3.10,<4.0
```

