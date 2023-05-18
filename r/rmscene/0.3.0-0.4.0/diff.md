# Comparing `tmp/rmscene-0.3.0.tar.gz` & `tmp/rmscene-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmscene-0.3.0.tar", max compression
+gzip compressed data, was "rmscene-0.4.0.tar", max compression
```

## Comparing `rmscene-0.3.0.tar` & `rmscene-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1068 2023-03-13 19:32:07.259406 rmscene-0.3.0/LICENSE
--rw-r--r--   0        0        0      438 2023-03-13 19:32:07.259406 rmscene-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      133 2023-03-13 19:32:07.259406 rmscene-0.3.0/src/rmscene/__init__.py
--rw-r--r--   0        0        0     1888 2023-03-13 19:32:07.259406 rmscene-0.3.0/src/rmscene/__main__.py
--rw-r--r--   0        0        0     3787 2023-03-13 19:32:07.259406 rmscene-0.3.0/src/rmscene/crdt_sequence.py
--rw-r--r--   0        0        0        0 2023-03-13 19:32:07.259406 rmscene-0.3.0/src/rmscene/py.typed
--rw-r--r--   0        0        0     5217 2023-03-13 19:32:07.259406 rmscene-0.3.0/src/rmscene/scene_items.py
--rw-r--r--   0        0        0    27387 2023-03-13 19:32:07.263406 rmscene-0.3.0/src/rmscene/scene_stream.py
--rw-r--r--   0        0        0     1581 2023-03-13 19:32:07.263406 rmscene-0.3.0/src/rmscene/scene_tree.py
--rw-r--r--   0        0        0     7822 2023-03-13 19:32:07.263406 rmscene-0.3.0/src/rmscene/tagged_block_common.py
--rw-r--r--   0        0        0     8352 2023-03-13 19:32:07.263406 rmscene-0.3.0/src/rmscene/tagged_block_reader.py
--rw-r--r--   0        0        0     5688 2023-03-13 19:32:07.263406 rmscene-0.3.0/src/rmscene/tagged_block_writer.py
--rw-r--r--   0        0        0     1676 2023-03-13 19:32:07.263406 rmscene-0.3.0/src/rmscene/text.py
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 rmscene-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-18 16:20:21.308008 rmscene-0.4.0/LICENSE
+-rw-r--r--   0        0        0      458 2023-05-18 16:20:21.308008 rmscene-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/__init__.py
+-rw-r--r--   0        0        0      524 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/__main__.py
+-rw-r--r--   0        0        0     3787 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/crdt_sequence.py
+-rw-r--r--   0        0        0        0 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/py.typed
+-rw-r--r--   0        0        0     3839 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/scene_items.py
+-rw-r--r--   0        0        0    29157 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/scene_stream.py
+-rw-r--r--   0        0        0     1581 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/scene_tree.py
+-rw-r--r--   0        0        0     7822 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/tagged_block_common.py
+-rw-r--r--   0        0        0     9312 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/tagged_block_reader.py
+-rw-r--r--   0        0        0     6141 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/tagged_block_writer.py
+-rw-r--r--   0        0        0     5731 2023-05-18 16:20:21.308008 rmscene-0.4.0/src/rmscene/text.py
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 rmscene-0.4.0/PKG-INFO
```

### Comparing `rmscene-0.3.0/LICENSE` & `rmscene-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rmscene-0.3.0/src/rmscene/crdt_sequence.py` & `rmscene-0.4.0/src/rmscene/crdt_sequence.py`

 * *Files identical despite different names*

### Comparing `rmscene-0.3.0/src/rmscene/scene_items.py` & `rmscene-0.4.0/src/rmscene/text.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,235 +1,185 @@
-"""Data structures for the contents of a scene."""
+"""Process text from remarkable scene files.
 
+"""
+
+from __future__ import annotations
+
+from collections.abc import Iterable
+from collections import defaultdict
 from dataclasses import dataclass, field
-import enum
 import logging
 import typing as tp
 
+from . import scene_items as si
 from .tagged_block_common import CrdtId, LwwValue
-from .crdt_sequence import CrdtSequence
-from .text import expand_text_items
-
+from .crdt_sequence import CrdtSequence, CrdtSequenceItem
 
 _logger = logging.getLogger(__name__)
 
 
-## Base class
-
-
-@dataclass
-class SceneItem:
-    """Base class for items stored in scene tree."""
-
-
-## Group
-
-
-@dataclass
-class Group(SceneItem):
-    """A Group represents a group of nested items.
-
-    Groups are used to represent layers.
-
-    node_id is the id that this sub-tree is stored as a "SceneTreeBlock".
-
-    children is a sequence of other SceneItems.
-
-    `anchor_id` refers to a text character which provides the anchor y-position
-    for this group. There are two values that seem to be special:
-    - `0xfffffffffffe` seems to be used for lines right at the top of the page?
-    - `0xffffffffffff` seems to be used for lines right at the bottom of the page?
-
-    """
-
-    node_id: CrdtId
-    children: CrdtSequence[SceneItem] = field(default_factory=CrdtSequence)
-    label: LwwValue[str] = LwwValue(CrdtId(0, 0), "")
-    visible: LwwValue[bool] = LwwValue(CrdtId(0, 0), True)
-
-    anchor_id: tp.Optional[LwwValue[CrdtId]] = None
-    anchor_type: tp.Optional[LwwValue[int]] = None
-    anchor_threshold: tp.Optional[LwwValue[float]] = None
-    anchor_origin_x: tp.Optional[LwwValue[float]] = None
-
-
-## Strokes
-
-
-@enum.unique
-class PenColor(enum.IntEnum):
-    """
-    Color index value.
-    """
-
-    # XXX list from remt pre-v6
-
-    BLACK = 0
-    GRAY = 1
-    WHITE = 2
+def expand_text_item(item: CrdtSequenceItem[str | int]) -> Iterable[CrdtSequenceItem[str] | CrdtSequenceItem[int]]:
+    """Expand TextItem into single-character TextItems.
 
-    YELLOW = 3
-    GREEN = 4
-    PINK = 5
+    Text is stored as strings in TextItems, each with an associated ID for the
+    block. This ID identifies the character at the start of the block. The
+    subsequent characters' IDs are implicit.
 
-    BLUE = 6
-    RED = 7
+    This function expands a TextItem into multiple single-character TextItems,
+    so that each character has an explicit ID.
 
-    GRAY_OVERLAP = 8
-
-
-@enum.unique
-class Pen(enum.IntEnum):
     """
-    Stroke pen id representing reMarkable tablet tools.
 
-    Tool examples: ballpoint, fineliner, highlighter or eraser.
-    """
+    if item.deleted_length > 0:
+        assert item.value == ""
+        chars = [""] * item.deleted_length
+        deleted_length = 1
+    elif isinstance(item.value, int):
+        yield item
+        return
+    else:
+        # Actually the value can be empty
+        # assert len(item.value) > 0
+        chars = item.value
+        deleted_length = 0
 
-    # XXX this list is from remt pre-v6
+    if not chars:
+        _logger.warning("Unexpected empty text item: %s", item)
+        return
 
-    BALLPOINT_1 = 2
-    BALLPOINT_2 = 15
-    CALIGRAPHY = 21
-    ERASER = 6
-    ERASER_AREA = 8
-    FINELINER_1 = 4
-    FINELINER_2 = 17
-    HIGHLIGHTER_1 = 5
-    HIGHLIGHTER_2 = 18
-    MARKER_1 = 3
-    MARKER_2 = 16
-    MECHANICAL_PENCIL_1 = 7
-    MECHANICAL_PENCIL_2 = 13
-    PAINTBRUSH_1 = 0
-    PAINTBRUSH_2 = 12
-    PENCIL_1 = 1
-    PENCIL_2 = 14
+    item_id = item.item_id
+    left_id = item.left_id
+    for c in chars[:-1]:
+        right_id = CrdtId(item_id.part1, item_id.part2 + 1)
+        yield CrdtSequenceItem(item_id, left_id, right_id, deleted_length, c)
+        left_id = item_id
+        item_id = right_id
+    yield CrdtSequenceItem(item_id, left_id, item.right_id, deleted_length, chars[-1])
 
-    @classmethod
-    def is_highlighter(cls, value: int) -> bool:
-        return value in (cls.HIGHLIGHTER_1, cls.HIGHLIGHTER_2)
 
-
-@dataclass
-class Point:
-    x: float
-    y: float
-    speed: int
-    direction: int
-    width: int
-    pressure: int
+def expand_text_items(items: Iterable[CrdtSequenceItem[str | int]]) -> Iterable[CrdtSequenceItem[str] | CrdtSequenceItem[int]]:
+    """Expand a sequence of TextItems into single-character TextItems."""
+    for item in items:
+        yield from expand_text_item(item)
 
 
 @dataclass
-class Line(SceneItem):
-    color: PenColor
-    tool: Pen
-    points: list[Point]
-    thickness_scale: float
-    starting_length: float
+class CrdtStr:
+    s: str = ""
+    i: list[CrdtId] = field(default_factory=list)
 
+    def __str__(self):
+        return self.s
 
-## Text
 
+@dataclass
+class TextSpan:
+    """Base class for text spans with formatting."""
+    contents: list[tp.Union["TextSpan", CrdtStr]]
 
-@enum.unique
-class TextFormat(enum.IntEnum):
-    """
-    Text format type.
-    """
 
-    PLAIN = 1
-    HEADING = 2
-    BOLD = 3
-    BULLET = 4
-    BULLET2 = 5
+class BoldSpan(TextSpan):
+    pass
 
 
-END_MARKER = CrdtId(0, 0)
+class ItalicSpan(TextSpan):
+    pass
 
 
 @dataclass
-class Text(SceneItem):
-    """Block of text.
+class Paragraph:
+    """Paragraph of text."""
+    contents: list[TextSpan]
+    start_id: CrdtId
+    style: LwwValue[si.ParagraphStyle]
 
-    `items` are a CRDT sequence of strings. The `item_id` for each string refers
-    to its first character; subsequent characters implicitly have sequential
-    ids.
-
-    `formats` are LWW values representing a mapping of character IDs to
-    `TextFormat` values. These formats apply to each line of text (until the
-    next newline).
+    def __str__(self):
+        return "".join(str(s) for s in self.contents)
 
-    `pos_x`, `pos_y` and `width` are dimensions for the text block.
-
-    """
 
-    items: CrdtSequence[str]
-    formats: dict[CrdtId, LwwValue[TextFormat]]
-    pos_x: float
-    pos_y: float
-    width: float
+@dataclass
+class TextDocument:
 
-    def formatted_lines_with_ids(self) -> tp.Iterator[tuple[TextFormat, str, list[CrdtId]]]:
-        """Extract lines of text with associated formatting and char ids.
+    contents: list[Paragraph]
 
-        Returns (format, line, char_ids) tuples.
+    @classmethod
+    def from_scene_item(cls, text: si.Text):
+        """Extract spans of text with associated formatting and char ids.
 
+        This uses the inline formatting introduced in v3.3.2.
         """
 
-        char_formats = {k: lww.value for k, lww in self.formats.items()}
-        if END_MARKER in char_formats:
-            current_format = char_formats[END_MARKER]
-        else:
-            current_format = TextFormat.PLAIN
+        char_formats = {k: lww.value for k, lww in text.styles.items()}
+        if si.END_MARKER not in char_formats:
+            char_formats[si.END_MARKER] = si.ParagraphStyle.PLAIN
 
         # Expand from strings to characters
-        char_items = CrdtSequence(expand_text_items(self.items.sequence_items()))
-
-        current_line = ""
-        current_ids = []
-        for k in char_items:
-            char = char_items[k]
-            assert len(char) <= 1
-            current_line += char
-            current_ids += [k]
-            if char == "\n":
-                yield (current_format, current_line, current_ids)
-                current_format = TextFormat.PLAIN
-                current_line = ""
-                current_ids = []
-            if k in char_formats:
-                current_format = char_formats[k]
-                if char != "\n":
-                    _logger.warning("format does not apply to whole line")
-
-        yield (current_format, current_line, current_ids)
-
-    def formatted_lines(self) -> tp.Iterator[tuple[TextFormat, str]]:
-        """Extract lines of text with associated formatting.
-
-        Returns (format, line) tuples.
-
-        """
-        for fmt, s, _ in self.formatted_lines_with_ids():
-            yield (fmt, s)
-
-
-## Glyph range
-
-
-@dataclass
-class Rectangle:
-    x: float
-    y: float
-    w: float
-    h: float
-
-
-@dataclass
-class GlyphRange(SceneItem):
-    start: int
-    length: int
-    text: str
-    color: PenColor
-    rectangles: list[Rectangle]
+        char_items = CrdtSequence(expand_text_items(text.items.sequence_items()))
+        keys = list(char_items)
+        last_linebreak = si.END_MARKER
+
+        span_start_codes = {
+            1: BoldSpan,
+            3: ItalicSpan,
+        }
+        span_end_codes = {
+            2: BoldSpan,
+            4: ItalicSpan,
+        }
+
+        def parse_paragraph_contents():
+            nonlocal last_linebreak
+            stack = [(None, [])]
+            k = None
+            done = False
+            while keys:
+                # If we've seen a newline character, only interested in
+                # span-closing format codes.
+                if done and char_items[keys[0]] not in (2, 4):
+                    break
+
+                k = keys.pop(0)
+                char = char_items[k]
+                if isinstance(char, int):
+                    if char in span_start_codes:
+                        span_type = span_start_codes[char]
+                        stack.append((span_type, []))
+                    elif char in span_end_codes:
+                        span_type, nested = stack.pop()
+                        if span_type is not span_end_codes[char]:
+                            _logger.error("Unexpected end of span at %s: got %s, expected %s",
+                                          k, span_end_codes[char], span_type)
+                        stack[-1][1].append(span_type(nested))
+                    else:
+                        _logger.warning("Unknown format code %d at %s!", char, k)
+                elif char == "\n":
+                    # End of paragraph
+                    done = True
+                    last_linebreak = k
+                else:
+                    assert len(char) <= 1
+                    _, contents = stack[-1]
+                    if not contents or not isinstance(contents[-1], CrdtStr):
+                        contents += [CrdtStr()]
+                    contents[-1].s += char
+                    contents[-1].i += [k]
+
+            if len(stack) > 1:
+                _logger.error("Unbalanced stack! %s", stack)
+
+            _, contents = stack[-1]
+            return contents
+
+        paragraphs = []
+        while keys:
+            style = text.styles.get(last_linebreak, LwwValue(CrdtId(0, 0), si.ParagraphStyle.PLAIN))
+            contents = parse_paragraph_contents()
+            p = Paragraph(contents, last_linebreak, style)
+            paragraphs += [p]
+
+        doc = cls(paragraphs)
+        return doc
+
+        # if k in char_formats:
+        #     current_format = char_formats[k]
+        #     if char != "\n":
+        #         _logger.warning("format does not apply to whole line")
```

### Comparing `rmscene-0.3.0/src/rmscene/scene_stream.py` & `rmscene-0.4.0/src/rmscene/scene_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from collections.abc import Iterable
 import math
 from uuid import UUID, uuid4
 from dataclasses import dataclass, replace, KW_ONLY
 import logging
 import typing as tp
 
+from packaging.version import Version
+
 from .tagged_block_common import CrdtId, LwwValue
 from .tagged_block_reader import TaggedBlockReader
 from .tagged_block_writer import TaggedBlockWriter
 from .crdt_sequence import CrdtSequence, CrdtSequenceItem
 from .scene_tree import SceneTree
 from . import scene_items as si
 
@@ -94,27 +96,35 @@
 
 @dataclass
 class MigrationInfoBlock(Block):
     BLOCK_TYPE: tp.ClassVar = 0x00
 
     migration_id: CrdtId
     is_device: bool
+    _unknown: bool = False
 
     @classmethod
     def from_stream(cls, stream: TaggedBlockReader) -> MigrationInfoBlock:
         "Parse migration info"
         _logger.debug("Reading %s", cls.__name__)
         migration_id = stream.read_id(1)
         is_device = stream.read_bool(2)
-        return MigrationInfoBlock(migration_id, is_device)
+        if stream.bytes_remaining_in_block():
+            unknown = stream.read_bool(3)
+        else:
+            unknown = False
+        return MigrationInfoBlock(migration_id, is_device, unknown)
 
     def to_stream(self, writer: TaggedBlockWriter):
         _logger.debug("Writing %s", type(self).__name__)
+        version = writer.options.get("version", Version("9.9.9"))
         writer.write_id(1, self.migration_id)
         writer.write_bool(2, self.is_device)
+        if version >= Version("3.2.2"):
+            writer.write_bool(3, self._unknown)
 
 
 @dataclass
 class TreeNodeBlock(Block):
     BLOCK_TYPE: tp.ClassVar = 0x02
 
     group: si.Group
@@ -166,33 +176,39 @@
         """Return (min_version, current_version) to use when writing."""
         return (0, 1)
 
     loads_count: int
     merges_count: int
     text_chars_count: int
     text_lines_count: int
+    _unknown: int = 0
 
     @classmethod
     def from_stream(cls, stream: TaggedBlockReader) -> PageInfoBlock:
         "Parse page info block"
         _logger.debug("Reading %s", cls.__name__)
         info = PageInfoBlock(
             loads_count=stream.read_int(1),
             merges_count=stream.read_int(2),
             text_chars_count=stream.read_int(3),
             text_lines_count=stream.read_int(4),
         )
+        if stream.bytes_remaining_in_block():
+            info._unknown = stream.read_int(5)
         return info
 
     def to_stream(self, writer: TaggedBlockWriter):
         _logger.debug("Writing %s", type(self).__name__)
         writer.write_int(1, self.loads_count)
         writer.write_int(2, self.merges_count)
         writer.write_int(3, self.text_chars_count)
         writer.write_int(4, self.text_lines_count)
+        version = writer.options.get("version", Version("9999"))
+        if version >= Version("3.2.2"):
+            writer.write_int(5, self._unknown)
 
 
 @dataclass
 class SceneTreeBlock(Block):
     BLOCK_TYPE: tp.ClassVar = 0x01
 
     # XXX not sure what the difference is
@@ -476,28 +492,29 @@
     BLOCK_TYPE: tp.ClassVar = 0x05
     ITEM_TYPE: tp.ClassVar = 0x03
 
     value: tp.Optional[si.Line]
 
     def version_info(self, writer: TaggedBlockWriter) -> tuple[int, int]:
         """Return (min_version, current_version) to use when writing."""
-        ver = writer.options.get("line_version", 2)
-        return (ver, ver)
+        version = writer.options.get("version", Version("9999"))
+        return (2, 2) if (version > Version("3.0")) else (1, 1)
 
     @classmethod
     def value_from_stream(cls, reader: TaggedBlockReader) -> si.Line:
         assert reader.current_block is not None
         version = reader.current_block.current_version
         value = line_from_stream(reader, version)
         return value
 
     def value_to_stream(self, writer: TaggedBlockWriter, value: si.Line):
         # XXX make sure this version ends up in block header
-        version = writer.options.get("line_version", 2)
-        line_to_stream(value, writer, version=version)
+        version = writer.options.get("version", Version("9999"))
+        line_version = 2 if (version > Version("3.0")) else 1
+        line_to_stream(value, writer, version=line_version)
 
 
 # XXX missing "PathItemBlock"? with ITEM_TYPE 0x04
 
 
 class SceneTextItemBlock(SceneItemBlock):
     BLOCK_TYPE: tp.ClassVar = 0x06
@@ -507,62 +524,80 @@
     def value_from_stream(cls, reader: TaggedBlockReader) -> tp.Any:
         return None
 
     def value_to_stream(self, writer: TaggedBlockWriter, value):
         pass
 
 
-def text_item_from_stream(stream: TaggedBlockReader) -> CrdtSequenceItem[str]:
+def text_item_from_stream(stream: TaggedBlockReader) -> CrdtSequenceItem[str | int]:
     with stream.read_subblock(0):
         item_id = stream.read_id(2)
         left_id = stream.read_id(3)
         right_id = stream.read_id(4)
         deleted_length = stream.read_int(5)
 
         if stream.has_subblock(6):
-            text = stream.read_string(6)
+            text, fmt = stream.read_string_with_format(6)
+            # It seems that formats are stored on empty strings, so it's one or the other
+            if fmt is not None:
+                if text:
+                    _logger.error("Unhandled combined text and format: %s, %s",
+                                  text, fmt)
+                value = fmt
+            else:
+                value = text
         else:
-            text = ""
+            value = ""
 
-    return CrdtSequenceItem(item_id, left_id, right_id, deleted_length, text)
+    return CrdtSequenceItem(item_id, left_id, right_id, deleted_length, value)
 
 
-def text_item_to_stream(item: CrdtSequenceItem[str], writer: TaggedBlockWriter):
+def text_item_to_stream(item: CrdtSequenceItem[str | int], writer: TaggedBlockWriter):
     with writer.write_subblock(0):
         writer.write_id(2, item.item_id)
         writer.write_id(3, item.left_id)
         writer.write_id(4, item.right_id)
         writer.write_int(5, item.deleted_length)
 
         if item.value:
-            writer.write_string(6, item.value)
+            if isinstance(item.value, str):
+                writer.write_string(6, item.value)
+            elif isinstance(item.value, int):
+                writer.write_string_with_format(6, "", item.value)
 
 
 def text_format_from_stream(
     stream: TaggedBlockReader,
-) -> tuple[CrdtId, LwwValue[si.TextFormat]]:
+) -> tuple[CrdtId, LwwValue[si.ParagraphStyle]]:
     # These are character ids, but not with an initial tag like other ids have.
     char_id = stream.data.read_crdt_id()
 
     # This seems to be the item ID for this format data? It doesn't appear
     # elsewhere in the file. Sometimes coincides with a character id but I don't
     # think it is referring to it.
     timestamp = stream.read_id(1)
 
     with stream.read_subblock(2):
         # XXX not sure what this is format?
         c = stream.data.read_uint8()
         assert c == 17
-        format_type = si.TextFormat(stream.data.read_uint8())
+        format_code = stream.data.read_uint8()
+        try:
+            format_type = si.ParagraphStyle(format_code)
+        except ValueError:
+            _logger.warning("Unrecognised text format code %d.", format_code)
+            _logger.debug("Unrecognised text format code %d at position %d.",
+                          format_code, stream.data.tell())
+            format_type = si.ParagraphStyle.PLAIN  # fallback
 
     return (char_id, LwwValue(timestamp, format_type))
 
 
 def text_format_to_stream(
-    char_id: CrdtId, value: LwwValue[si.TextFormat], writer: TaggedBlockWriter
+    char_id: CrdtId, value: LwwValue[si.ParagraphStyle], writer: TaggedBlockWriter
 ):
     format_type = value.value
 
     writer.data.write_crdt_id(char_id)
     writer.write_id(1, value.timestamp)
     with writer.write_subblock(2):
         # XXX not sure what this is format?
@@ -612,15 +647,15 @@
             pos_y = stream.data.read_float64()
 
         # "width" from ddvk
         width = stream.read_float(4)
 
         value = si.Text(
             items=CrdtSequence(text_items),
-            formats=text_formats,
+            styles=text_formats,
             pos_x=pos_x,
             pos_y=pos_y,
             width=width
         )
         return RootTextBlock(block_id, value)
 
     def to_stream(self, writer: TaggedBlockWriter):
@@ -634,15 +669,15 @@
             with writer.write_subblock(1):
                 with writer.write_subblock(1):
                     writer.data.write_varuint(len(text_items))
                     for item in text_items:
                         text_item_to_stream(item, writer)
 
             # Formatting
-            text_formats = self.value.formats
+            text_formats = self.value.styles
             with writer.write_subblock(2):
                 with writer.write_subblock(1):
                     writer.data.write_varuint(len(text_formats))
                     for key, item in text_formats.items():
                         text_format_to_stream(key, item, writer)
 
         # Last section
@@ -698,14 +733,16 @@
 
 def write_blocks(
     data: tp.BinaryIO, blocks: Iterable[Block], options: tp.Optional[dict] = None
 ):
     """
     Write blocks to file.
     """
+    if options is not None and "version" in options:
+        options["version"] = Version(options["version"])
     stream = TaggedBlockWriter(data, options=options)
     stream.write_header()
     for block in blocks:
         _write_block(stream, block)
 
 
 def build_tree(tree: SceneTree, blocks: Iterable[Block]):
@@ -795,16 +832,16 @@
                     item_id=CrdtId(1, 16),
                     left_id=CrdtId(0, 0),
                     right_id=CrdtId(0, 0),
                     deleted_length=0,
                     value=text,
                 )
             ]),
-            formats={
-                CrdtId(0, 0): LwwValue(timestamp=CrdtId(1, 15), value=si.TextFormat.PLAIN),
+            styles={
+                CrdtId(0, 0): LwwValue(timestamp=CrdtId(1, 15), value=si.ParagraphStyle.PLAIN),
             },
             pos_x=-468.0,
             pos_y=234.0,
             width=936.0,
         )
     )
```

### Comparing `rmscene-0.3.0/src/rmscene/scene_tree.py` & `rmscene-0.4.0/src/rmscene/scene_tree.py`

 * *Files identical despite different names*

### Comparing `rmscene-0.3.0/src/rmscene/tagged_block_common.py` & `rmscene-0.4.0/src/rmscene/tagged_block_common.py`

 * *Files identical despite different names*

### Comparing `rmscene-0.3.0/src/rmscene/tagged_block_reader.py` & `rmscene-0.4.0/src/rmscene/tagged_block_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,14 +197,16 @@
             # Discard the rest
             remaining = i0 + length - i1
             excess = self.data.read_bytes(remaining)
             block_info.extra_data = excess
             _logger.debug(
                 "Excess bytes:\n %s",
                 "\n".join(excess[i : i + 32].hex() for i in range(0, len(excess), 32)),
+                stack_info=True,
+                stacklevel=4,
             )
 
     ## Higher level constructs
 
     def read_lww_bool(self, index: int) -> LwwValue[bool]:
         "Read a LWW bool."
         with self.read_subblock(index):
@@ -251,7 +253,29 @@
             assert string_length + 2 <= block_info.size
             b = self.data.read_bytes(string_length)
             string = b.decode()
             if len(b) != len(string):
                 _logger.debug("read_string: decoded %r (%d) to %r (%d)",
                               b, len(b), string, len(string))
             return string
+
+    def read_string_with_format(self, index: int) -> tuple[str, tp.Optional[int]]:
+        """Read a string block with formatting."""
+        with self.read_subblock(index) as block_info:
+            string_length = self.data.read_varuint()
+            # XXX not sure if this is right meaning?
+            is_ascii = self.data.read_bool()
+            assert is_ascii == 1
+            assert string_length + 2 <= block_info.size
+            b = self.data.read_bytes(string_length)
+            string = b.decode()
+            if len(b) != len(string):
+                _logger.debug("read_string: decoded %r (%d) to %r (%d)",
+                              b, len(b), string, len(string))
+
+            if self.data.check_tag(2, TagType.Byte4):
+                # We have a format code
+                fmt = self.read_int(2)
+            else:
+                fmt = None
+
+            return string, fmt
```

### Comparing `rmscene-0.3.0/src/rmscene/tagged_block_writer.py` & `rmscene-0.4.0/src/rmscene/tagged_block_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,8 +170,19 @@
         """Write a standard string block."""
         with self.write_subblock(index):
             b = value.encode()
             bytes_length = len(b)
             is_ascii = True  # XXX not sure if this is right meaning?
             self.data.write_varuint(bytes_length)
             self.data.write_bool(is_ascii)
-            self.data.write_bytes(value.encode())
+            self.data.write_bytes(b)
+
+    def write_string_with_format(self, index: int, text: str, fmt: int):
+        """Write a string block with formatting."""
+        with self.write_subblock(index):
+            b = text.encode()
+            bytes_length = len(b)
+            is_ascii = True  # XXX not sure if this is right meaning?
+            self.data.write_varuint(bytes_length)
+            self.data.write_bool(is_ascii)
+            self.data.write_bytes(b)
+            self.write_int(2, fmt)
```

### Comparing `rmscene-0.3.0/PKG-INFO` & `rmscene-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: rmscene
-Version: 0.3.0
+Version: 0.4.0
 Summary: Read v6 .rm files from the reMarkable tablet
 Home-page: https://github.com/ricklupton/rmscene
 License: MIT
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: packaging (>=23.0,<24.0)
 Project-URL: Repository, https://github.com/ricklupton/rmscene
```

