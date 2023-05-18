# Comparing `tmp/interactions-lavalink-1.0.0.tar.gz` & `tmp/interactions-lavalink-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactions-lavalink-1.0.0.tar", last modified: Wed Dec 28 17:21:41 2022, max compression
+gzip compressed data, was "interactions-lavalink-2.0.0.tar", last modified: Thu May 18 14:59:55 2023, max compression
```

## Comparing `interactions-lavalink-1.0.0.tar` & `interactions-lavalink-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 17:21:41.796014 interactions-lavalink-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-28 17:21:28.000000 interactions-lavalink-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2022-12-28 17:21:41.796014 interactions-lavalink-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2022-12-28 17:21:28.000000 interactions-lavalink-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 17:21:41.792014 interactions-lavalink-1.0.0/interactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 17:21:41.792014 interactions-lavalink-1.0.0/interactions/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 17:21:41.792014 interactions-lavalink-1.0.0/interactions/ext/lavalink/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-28 17:21:28.000000 interactions-lavalink-1.0.0/interactions/ext/lavalink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-28 17:21:28.000000 interactions-lavalink-1.0.0/interactions/ext/lavalink/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2022-12-28 17:21:28.000000 interactions-lavalink-1.0.0/interactions/ext/lavalink/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2022-12-28 17:21:28.000000 interactions-lavalink-1.0.0/interactions/ext/lavalink/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 17:21:41.796014 interactions-lavalink-1.0.0/interactions_lavalink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2022-12-28 17:21:41.000000 interactions-lavalink-1.0.0/interactions_lavalink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2022-12-28 17:21:41.000000 interactions-lavalink-1.0.0/interactions_lavalink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 17:21:41.000000 interactions-lavalink-1.0.0/interactions_lavalink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-28 17:21:41.000000 interactions-lavalink-1.0.0/interactions_lavalink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-28 17:21:41.000000 interactions-lavalink-1.0.0/interactions_lavalink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2022-12-28 17:21:28.000000 interactions-lavalink-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-28 17:21:41.796014 interactions-lavalink-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2022-12-28 17:21:28.000000 interactions-lavalink-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:59:55.198724 interactions-lavalink-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-18 14:59:55.198724 interactions-lavalink-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:59:55.194724 interactions-lavalink-2.0.0/interactions_lavalink/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/interactions_lavalink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/interactions_lavalink/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/interactions_lavalink/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/interactions_lavalink/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:59:55.198724 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-18 14:59:55.000000 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-18 14:59:55.000000 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:59:55.000000 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-18 14:59:55.000000 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 14:59:55.000000 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:59:55.198724 interactions-lavalink-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/setup.py
```

### Comparing `interactions-lavalink-1.0.0/LICENSE` & `interactions-lavalink-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interactions-lavalink-1.0.0/PKG-INFO` & `interactions-lavalink-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: interactions-lavalink
-Version: 1.0.0
-Summary: Lavalink and voice support for interactions.py
-Home-page: https://github.com/interactions-py/interactions-lavalink
+Version: 2.0.0
+Summary: Lavalink support for interactions.py
+Home-page: https://github.com/interactions-py/lavalink
 Author: Damego
 Author-email: damego.dev@gmail.com
-License: GPL-3.0 License
+License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # interactions-lavalink
 
 ## Installation
 
@@ -41,105 +40,104 @@
 
 Main file:
 ```python
 from interactions import Client
 
 
 # Creating bot variable
-client = Client(...)
+client = Client()
 
 # Loading your extension
 client.load("exts.music")
 
 # Starting bot
-client.start()
+client.start("TOKEN")
 ```
 
 Extension file: `exts/music.py`
 ```python
-from interactions import Extension, extension_command, extension_listener, option, CommandContext, VoiceState
-from interactions.ext.lavalink import Lavalink
+from interactions import Extension, SlashContext, listen, slash_command, slash_option
+
+from interactions_lavalink import Lavalink
+from interactions_lavalink.events import TrackStart
 
 
 class Music(Extension):
     def __init__(self, client):
         self.client = client
-        self.lavalink: Lavalink = None
+        self.lavalink: Lavalink | None = None
 
-    @extension_listener()
-    async def on_start(self):
-        # Initialize lavalink instance
+    @listen()
+    async def on_startup(self):
+        # Initializing lavalink instance on bot startup
         self.lavalink: Lavalink = Lavalink(self.client)
 
-        # Connect to lavalink server
+        # Connecting to local lavalink server
         self.lavalink.add_node("127.0.0.1", 43421, "your_password", "eu")
 
-    @extension_command()
-    @option()
-    async def play(self, ctx: CommandContext, query: str):
+    @listen()
+    async def on_track_start(self, event: TrackStart):
+        print("Track started", event.track.title)
+
+    @slash_command()
+    @slash_option("query", "The search query or url", opt_type=3, required=True)
+    async def play(self, ctx: SlashContext, query: str):
         await ctx.defer()
 
         # Getting user's voice state
-        voice_state: VoiceState = ctx.author.voice_state
-        if not voice_state or not voice_state.joined:
+        voice_state = ctx.author.voice
+        if not voice_state or not voice_state.channel:
             return await ctx.send("You're not connected to the voice channel!")
 
         # Connecting to voice channel and getting player instance
-        player = await self.lavalink.connect(voice_state.guild_id, voice_state.channel_id)
-
+        player = await self.lavalink.connect(voice_state.guild.id, voice_state.channel.id)
         # Getting tracks from youtube
         tracks = await player.search_youtube(query)
-        # Selecting first founded track
         track = tracks[0]
         # Adding track to the queue
         player.add(requester=int(ctx.author.id), track=track)
 
-        # Check if already playing
+        # Check if player is already playing
         if player.is_playing:
             return await ctx.send(f"Added to queue: `{track.title}`")
 
         # Starting playing track
         await player.play()
         await ctx.send(f"Now playing: `{track.title}`")
 
-    @extension_command()
-    async def leave(self, ctx: CommandContext):
-        # Disconnect from voice channel and remove player
-        await self.lavalink.disconnect(ctx.guild_id)
+    @slash_command()
+    async def leave(self, ctx: SlashContext):
+        # Disconnecting from voice channel
+        await self.lavalink.disconnect(ctx.guild.id)
 
         await ctx.send("Disconnected", ephemeral=True)
-
-
-def setup(client):
-    Music(client)
-
 ```
 
 ## Events
-To listen lavalink event you have to use either `@bot.event` or `@extension_listener` decorator.
+To listen lavalink event you have to use `@listen` decorator.
 
 ```python
-from interactions import Extension, extension_listener
-
-import lavalink
+from interactions import Extension, listen
+from interactions_lavalink import TrackStart, TrackEnd, QueueEnd
 
 class MusicExt(Extension):
     ... # Some your cool music commands
 
     # There are many useful events for you. You can use other events if you want it.
-    @extension_listener()
-    async def on_track_start(self, event: lavalink.TrackStartEvent):
+    @listen()
+    async def on_track_start(self, event: TrackStart):
         """Fires when track starts"""
+        print(f"Track {event.track.title} started")
 
-    @extension_listener()
-    async def on_track_end(self, event: lavalink.TrackEndEvent):
+    @listen()
+    async def on_track_end(self, event: TrackEnd):
         """Fires when track ends"""
 
-    @extension_listener()
-    async def on_queue_end(self, event: lavalink.QueueEndEvent):
+    @listen()
+    async def on_queue_end(self, event: QueueEnd):
         """Fires when queue ends"""
 
 ```
 
 More events you could find in the `lavalink.py` documentation
 
 ## Documentation
```

### Comparing `interactions-lavalink-1.0.0/README.md` & `interactions-lavalink-2.0.0/interactions_lavalink.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: interactions-lavalink
+Version: 2.0.0
+Summary: Lavalink support for interactions.py
+Home-page: https://github.com/interactions-py/lavalink
+Author: Damego
+Author-email: damego.dev@gmail.com
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # interactions-lavalink
 
 ## Installation
 
 Download ext via `pip install --upgrade interactions-lavalink`
 
 ## Configuring own lavalink server
@@ -17,105 +40,104 @@
 
 Main file:
 ```python
 from interactions import Client
 
 
 # Creating bot variable
-client = Client(...)
+client = Client()
 
 # Loading your extension
 client.load("exts.music")
 
 # Starting bot
-client.start()
+client.start("TOKEN")
 ```
 
 Extension file: `exts/music.py`
 ```python
-from interactions import Extension, extension_command, extension_listener, option, CommandContext, VoiceState
-from interactions.ext.lavalink import Lavalink
+from interactions import Extension, SlashContext, listen, slash_command, slash_option
+
+from interactions_lavalink import Lavalink
+from interactions_lavalink.events import TrackStart
 
 
 class Music(Extension):
     def __init__(self, client):
         self.client = client
-        self.lavalink: Lavalink = None
+        self.lavalink: Lavalink | None = None
 
-    @extension_listener()
-    async def on_start(self):
-        # Initialize lavalink instance
+    @listen()
+    async def on_startup(self):
+        # Initializing lavalink instance on bot startup
         self.lavalink: Lavalink = Lavalink(self.client)
 
-        # Connect to lavalink server
+        # Connecting to local lavalink server
         self.lavalink.add_node("127.0.0.1", 43421, "your_password", "eu")
 
-    @extension_command()
-    @option()
-    async def play(self, ctx: CommandContext, query: str):
+    @listen()
+    async def on_track_start(self, event: TrackStart):
+        print("Track started", event.track.title)
+
+    @slash_command()
+    @slash_option("query", "The search query or url", opt_type=3, required=True)
+    async def play(self, ctx: SlashContext, query: str):
         await ctx.defer()
 
         # Getting user's voice state
-        voice_state: VoiceState = ctx.author.voice_state
-        if not voice_state or not voice_state.joined:
+        voice_state = ctx.author.voice
+        if not voice_state or not voice_state.channel:
             return await ctx.send("You're not connected to the voice channel!")
 
         # Connecting to voice channel and getting player instance
-        player = await self.lavalink.connect(voice_state.guild_id, voice_state.channel_id)
-
+        player = await self.lavalink.connect(voice_state.guild.id, voice_state.channel.id)
         # Getting tracks from youtube
         tracks = await player.search_youtube(query)
-        # Selecting first founded track
         track = tracks[0]
         # Adding track to the queue
         player.add(requester=int(ctx.author.id), track=track)
 
-        # Check if already playing
+        # Check if player is already playing
         if player.is_playing:
             return await ctx.send(f"Added to queue: `{track.title}`")
 
         # Starting playing track
         await player.play()
         await ctx.send(f"Now playing: `{track.title}`")
 
-    @extension_command()
-    async def leave(self, ctx: CommandContext):
-        # Disconnect from voice channel and remove player
-        await self.lavalink.disconnect(ctx.guild_id)
+    @slash_command()
+    async def leave(self, ctx: SlashContext):
+        # Disconnecting from voice channel
+        await self.lavalink.disconnect(ctx.guild.id)
 
         await ctx.send("Disconnected", ephemeral=True)
-
-
-def setup(client):
-    Music(client)
-
 ```
 
 ## Events
-To listen lavalink event you have to use either `@bot.event` or `@extension_listener` decorator.
+To listen lavalink event you have to use `@listen` decorator.
 
 ```python
-from interactions import Extension, extension_listener
-
-import lavalink
+from interactions import Extension, listen
+from interactions_lavalink import TrackStart, TrackEnd, QueueEnd
 
 class MusicExt(Extension):
     ... # Some your cool music commands
 
     # There are many useful events for you. You can use other events if you want it.
-    @extension_listener()
-    async def on_track_start(self, event: lavalink.TrackStartEvent):
+    @listen()
+    async def on_track_start(self, event: TrackStart):
         """Fires when track starts"""
+        print(f"Track {event.track.title} started")
 
-    @extension_listener()
-    async def on_track_end(self, event: lavalink.TrackEndEvent):
+    @listen()
+    async def on_track_end(self, event: TrackEnd):
         """Fires when track ends"""
 
-    @extension_listener()
-    async def on_queue_end(self, event: lavalink.QueueEndEvent):
+    @listen()
+    async def on_queue_end(self, event: QueueEnd):
         """Fires when queue ends"""
 
 ```
 
 More events you could find in the `lavalink.py` documentation
 
 ## Documentation
```

### Comparing `interactions-lavalink-1.0.0/interactions/ext/lavalink/extension.py` & `interactions-lavalink-2.0.0/interactions_lavalink/extension.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-from typing import Union
-
+import lavalink.events
+from interactions import Client, Snowflake_Type, to_snowflake
+from interactions.api.events.base import RawGatewayEvent
 from lavalink import Client as LavalinkClient
-from lavalink import Event as BaseLavalinkEvent
-
-from interactions import Channel, Client, Guild, OpCodeType, Snowflake
 
+from . import events
 from .player import Player
 
-__all__ = ("Lavalink", "setup")
+__all__ = ("Lavalink",)
 
 
 class Lavalink:
     def __init__(self, bot: Client):
         self._bot: Client = bot
-        self.client: LavalinkClient = None
+        self.client: LavalinkClient | None = None
 
-        if bot.me is not None:
-            self.__init_lavalink()
+        # Not an Extension so listen decorator can't be used
+        self._bot.listen()(self.__on_raw_voice_state_update)
+        self._bot.listen()(self.__on_raw_voice_server_update)
+
+    async def __on_raw_voice_state_update(self, event: RawGatewayEvent):
+        await self.client.voice_update_handler({"t": "VOICE_STATE_UPDATE", "d": event.data})
 
-        self._bot._websocket._dispatch.register(self.__raw_socket_create, "raw_socket_create")
+    async def __on_raw_voice_server_update(self, event: RawGatewayEvent):
+        await self.client.voice_update_handler({"t": "VOICE_SERVER_UPDATE", "d": event.data})
 
     def add_node(
         self,
         host: str,
         port: int,
         password: str,
         region: str,
@@ -46,123 +50,78 @@
             name=name,
             reconnect_attempts=reconnect_attempts,
             filters=filters,
             ssl=ssl,
         )
 
     def __init_lavalink(self):
-        self.client = LavalinkClient(int(self._bot.me.id), player=Player)
-        self.client.add_event_hook(self.__lavalink_event)
+        self.client = LavalinkClient(int(self._bot.user.id), player=Player)
+        self.client.add_event_hook(self._dispatch_lavalink_event)
 
-    def get_player(self, guild_id: Union[Guild, Snowflake, str, int]) -> Player:
+    def get_player(self, guild_id: Snowflake_Type) -> Player | None:
         """
-        :param Union[Guild, Snowflake, str, int] guild_id: The ID of the guild
-        :return: Founded player
-        :rtype: Player
-        """
-        _guild_id = int(guild_id.id if isinstance(guild_id, Guild) else guild_id)
-
-        player: Player = self.client.player_manager.get(_guild_id)
+        Gets guild's current player.
 
-        return player
+        :param Snowflake_Type guild_id: The ID of the guild
+        :return: Player, if any.
+        """
+        return self.client.player_manager.get(to_snowflake(guild_id))
 
-    def create_player(self, guild_id: Union[Guild, Snowflake, str, int]) -> Player:
+    def create_player(self, guild_id: Snowflake_Type) -> Player:
         """
-        :param Union[Guild, Snowflake, str, int] guild_id: The ID of the guild
+        Creates a new player for the guild
+
+        :param Snowflake_Type guild_id: The ID of the guild
         :return: Created player
-        :rtype: Player
         """
-        _guild_id = int(guild_id.id if isinstance(guild_id, Guild) else guild_id)
-
-        player = self.client.player_manager.create(_guild_id)
+        player = self.client.player_manager.create(to_snowflake(guild_id))
         player._bot = self._bot
 
-        return player
+        return player  # type: ignore
 
     async def connect(
         self,
-        guild_id: Union[Guild, Snowflake, str, int],
-        channel_id: Union[Channel, Snowflake, str, int],
+        guild_id: Snowflake_Type,
+        channel_id: Snowflake_Type,
         self_deaf: bool = False,
         self_mute: bool = False,
     ) -> Player:
         """
         Connects to voice channel and creates player.
 
-        :param Union[Snowflake, int, str] guild_id: The guild id to connect.
-        :param Union[Snowflake, int, str] channel_id: The channel id to connect.
+        :param Snowflake_Type guild_id: The guild id to connect.
+        :param Snowflake_Type channel_id: The channel id to connect.
         :param bool self_deaf: Whether bot is self deafened
         :param bool self_mute: Whether bot is self muted
         :return: Created guild player.
         :rtype: Player
         """
-        _guild_id = int(guild_id.id if isinstance(guild_id, Guild) else guild_id)
-        _channel_id = int(channel_id.id if isinstance(channel_id, Channel) else channel_id)
-        await self.__update_voice_state(_guild_id, _channel_id, self_deaf, self_mute)
+        _guild_id = to_snowflake(guild_id)
+
+        websocket = self._bot.get_guild_websocket(_guild_id)
+        await websocket.voice_state_update(
+            _guild_id, to_snowflake(channel_id), muted=self_mute, deafened=self_deaf
+        )
 
-        player = self.get_player(_guild_id)
-        if player is None:
-            player = self.create_player(_guild_id)
-        return player
+        return self.get_player(_guild_id) or self.create_player(_guild_id)
 
-    async def disconnect(self, guild_id: Union[Guild, Snowflake, str, int]):
+    async def disconnect(self, guild_id: Snowflake_Type):
         """
-        :param Union[Snowflake, int, str] guild_id: The guild id to disconnect from.
+        :param Snowflake_Type guild_id: The guild id to disconnect from.
         """
-        _guild_id = int(guild_id.id if isinstance(guild_id, Guild) else guild_id)
+        _guild_id = to_snowflake(guild_id)
+        websocket = self._bot.get_guild_websocket(_guild_id)
+        await websocket.voice_state_update(_guild_id, None)  # type: ignore
 
-        await self.__update_voice_state(_guild_id)
         await self.client.player_manager.destroy(_guild_id)
 
-    async def __lavalink_event(self, event: BaseLavalinkEvent):
-        event_name: str = self._get_event_name(event.__class__.__name__)
-
-        self._bot._websocket._dispatch.dispatch(event_name, event)
-
-    @staticmethod
-    def _get_event_name(event_name: str) -> str:
-        _event_name = event_name.removesuffix("Event")
-        for char in _event_name:
-            if char.isupper():
-                _event_name = _event_name.replace(char, f"_{char.lower()}", 1)
-        return f"on{_event_name}"
+    async def _dispatch_lavalink_event(self, event: lavalink.events.Event):
+        event_cls = getattr(events, event.__class__.__name__.removesuffix("Event"))
+        event_ins = event_cls(event)
+        self._bot.dispatch(event_ins)
 
     async def __raw_socket_create(self, name: str, data: dict):
         if name not in {"VOICE_STATE_UPDATE", "VOICE_SERVER_UPDATE"}:
             return
 
         _data: dict = {"t": name, "d": data}
         await self.client.voice_update_handler(_data)
-
-    async def __update_voice_state(
-        self,
-        guild_id: int,
-        channel_id: int = None,
-        self_deaf: bool = None,
-        self_mute: bool = None,
-    ):
-        """
-        Sends VOICE_STATE packet to websocket.
-
-        :param int guild_id: The guild id.
-        :param int channel_id: The channel id.
-        :param bool self_deaf: Whether bot is self deafened
-        :param bool self_mute: Whether bot is self muted
-        """
-        payload = {
-            "op": OpCodeType.VOICE_STATE,
-            "d": {
-                "guild_id": str(guild_id),
-                "channel_id": str(channel_id) if channel_id is not None else None,
-            },
-        }
-
-        if self_deaf is not None:
-            payload["d"]["self_deaf"] = self_deaf
-        if self_mute is not None:
-            payload["d"]["self_mute"] = self_mute
-
-        await self._bot._websocket._send_packet(payload)
-
-
-def setup(bot: Client):
-    return Lavalink(bot)
```

### Comparing `interactions-lavalink-1.0.0/interactions/ext/lavalink/player.py` & `interactions-lavalink-2.0.0/interactions_lavalink/player.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from typing import List
 
-from lavalink import AudioTrack, DefaultPlayer
-
 from interactions import Client
+from lavalink import AudioTrack, DefaultPlayer
 
 __all__ = ("Player",)
 
 
 class Player(DefaultPlayer):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self._bot: Client = None
+        self._bot: Client | None = None
 
     async def search_youtube(self, query: str) -> List[AudioTrack]:
         res = await self.node.get_tracks(f"ytsearch: {query}")
         return res.tracks
 
     async def search_soundcloud(self, query: str) -> List[AudioTrack]:
         res = await self.node.get_tracks(f"scsearch: {query}")
```

### Comparing `interactions-lavalink-1.0.0/interactions_lavalink.egg-info/PKG-INFO` & `interactions-lavalink-2.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: interactions-lavalink
-Version: 1.0.0
-Summary: Lavalink and voice support for interactions.py
-Home-page: https://github.com/interactions-py/interactions-lavalink
-Author: Damego
-Author-email: damego.dev@gmail.com
-License: GPL-3.0 License
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # interactions-lavalink
 
 ## Installation
 
 Download ext via `pip install --upgrade interactions-lavalink`
 
 ## Configuring own lavalink server
@@ -41,105 +17,104 @@
 
 Main file:
 ```python
 from interactions import Client
 
 
 # Creating bot variable
-client = Client(...)
+client = Client()
 
 # Loading your extension
 client.load("exts.music")
 
 # Starting bot
-client.start()
+client.start("TOKEN")
 ```
 
 Extension file: `exts/music.py`
 ```python
-from interactions import Extension, extension_command, extension_listener, option, CommandContext, VoiceState
-from interactions.ext.lavalink import Lavalink
+from interactions import Extension, SlashContext, listen, slash_command, slash_option
+
+from interactions_lavalink import Lavalink
+from interactions_lavalink.events import TrackStart
 
 
 class Music(Extension):
     def __init__(self, client):
         self.client = client
-        self.lavalink: Lavalink = None
+        self.lavalink: Lavalink | None = None
 
-    @extension_listener()
-    async def on_start(self):
-        # Initialize lavalink instance
+    @listen()
+    async def on_startup(self):
+        # Initializing lavalink instance on bot startup
         self.lavalink: Lavalink = Lavalink(self.client)
 
-        # Connect to lavalink server
+        # Connecting to local lavalink server
         self.lavalink.add_node("127.0.0.1", 43421, "your_password", "eu")
 
-    @extension_command()
-    @option()
-    async def play(self, ctx: CommandContext, query: str):
+    @listen()
+    async def on_track_start(self, event: TrackStart):
+        print("Track started", event.track.title)
+
+    @slash_command()
+    @slash_option("query", "The search query or url", opt_type=3, required=True)
+    async def play(self, ctx: SlashContext, query: str):
         await ctx.defer()
 
         # Getting user's voice state
-        voice_state: VoiceState = ctx.author.voice_state
-        if not voice_state or not voice_state.joined:
+        voice_state = ctx.author.voice
+        if not voice_state or not voice_state.channel:
             return await ctx.send("You're not connected to the voice channel!")
 
         # Connecting to voice channel and getting player instance
-        player = await self.lavalink.connect(voice_state.guild_id, voice_state.channel_id)
-
+        player = await self.lavalink.connect(voice_state.guild.id, voice_state.channel.id)
         # Getting tracks from youtube
         tracks = await player.search_youtube(query)
-        # Selecting first founded track
         track = tracks[0]
         # Adding track to the queue
         player.add(requester=int(ctx.author.id), track=track)
 
-        # Check if already playing
+        # Check if player is already playing
         if player.is_playing:
             return await ctx.send(f"Added to queue: `{track.title}`")
 
         # Starting playing track
         await player.play()
         await ctx.send(f"Now playing: `{track.title}`")
 
-    @extension_command()
-    async def leave(self, ctx: CommandContext):
-        # Disconnect from voice channel and remove player
-        await self.lavalink.disconnect(ctx.guild_id)
+    @slash_command()
+    async def leave(self, ctx: SlashContext):
+        # Disconnecting from voice channel
+        await self.lavalink.disconnect(ctx.guild.id)
 
         await ctx.send("Disconnected", ephemeral=True)
-
-
-def setup(client):
-    Music(client)
-
 ```
 
 ## Events
-To listen lavalink event you have to use either `@bot.event` or `@extension_listener` decorator.
+To listen lavalink event you have to use `@listen` decorator.
 
 ```python
-from interactions import Extension, extension_listener
-
-import lavalink
+from interactions import Extension, listen
+from interactions_lavalink import TrackStart, TrackEnd, QueueEnd
 
 class MusicExt(Extension):
     ... # Some your cool music commands
 
     # There are many useful events for you. You can use other events if you want it.
-    @extension_listener()
-    async def on_track_start(self, event: lavalink.TrackStartEvent):
+    @listen()
+    async def on_track_start(self, event: TrackStart):
         """Fires when track starts"""
+        print(f"Track {event.track.title} started")
 
-    @extension_listener()
-    async def on_track_end(self, event: lavalink.TrackEndEvent):
+    @listen()
+    async def on_track_end(self, event: TrackEnd):
         """Fires when track ends"""
 
-    @extension_listener()
-    async def on_queue_end(self, event: lavalink.QueueEndEvent):
+    @listen()
+    async def on_queue_end(self, event: QueueEnd):
         """Fires when queue ends"""
 
 ```
 
 More events you could find in the `lavalink.py` documentation
 
 ## Documentation
```

### Comparing `interactions-lavalink-1.0.0/setup.py` & `interactions-lavalink-2.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,37 @@
-import re
 from codecs import open
+from pathlib import Path
 
-from setuptools import setup
+from setuptools import setup, find_packages
+import tomli
 
-# Package information
-AUTHOR = "Damego"
-AUTHOR_EMAIL = "damego.dev@gmail.com"
-DESCRIPTION = "Lavalink and voice support for interactions.py"
-PROJECT_NAME = "interactions-lavalink"
-MAIN_PACKAGE_NAME = "interactions.ext.lavalink"
-URL = "https://github.com/interactions-py/interactions-lavalink"
-
-with open("README.md", "r", encoding="utf-8") as f:
-    README = f.read()
-
-with open("interactions/ext/lavalink/base.py") as fp:
-    VERSION = re.search('__version__ = "([^"]+)"', fp.read())[1]
+with open("pyproject.toml", "rb") as f:
+    pyproject = tomli.load(f)
 
 setup(
-    name=PROJECT_NAME,
-    version=VERSION,
-    author=AUTHOR,
-    author_email=AUTHOR_EMAIL,
-    description=DESCRIPTION,
+    name=pyproject["tool"]["poetry"]["name"],
+    version=pyproject["tool"]["poetry"]["version"],
+    author="Damego",
+    author_email="damego.dev@gmail.com",
+    description=pyproject["tool"]["poetry"]["description"],
     include_package_data=True,
-    install_requires=["discord-py-interactions>=4.3.2", "lavalink~=4.0.1"],
-    license="GPL-3.0 License",
-    long_description=README,
+    install_requires=["interactions.py>=5.0.0,<6.0.0", "lavalink>=4.0.0,<5.0.0"],
+    license=pyproject["tool"]["poetry"]["license"],
+    long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
-    url=URL,
-    packages=["interactions.ext.lavalink"],
-    python_requires=">=3.8",
+    url="https://github.com/interactions-py/lavalink",
+    packages=find_packages(),
+    python_requires=">=3.10",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Internet",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries",
         "Topic :: Utilities",
-    ],
+    ]
 )
```

