# Comparing `tmp/dice-3.1.2.tar.gz` & `tmp/dice-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dice-3.1.2.tar", last modified: Wed Apr  7 22:01:43 2021, max compression
+gzip compressed data, was "dice-4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dice-3.1.2.tar` & `dice-4.0.0.tar`

### file list

```diff
@@ -1,27 +1,20 @@
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-04-07 22:01:43.427116 dice-3.1.2/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    11238 2021-04-07 22:01:43.427116 dice-3.1.2/PKG-INFO
--rw-r--r--   0 caleb     (1000) caleb     (1000)     8549 2021-01-02 01:45:01.000000 dice-3.1.2/README.rst
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-04-07 22:01:43.423783 dice-3.1.2/dice/
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1739 2021-04-07 21:55:21.000000 dice-3.1.2/dice/__init__.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      169 2021-01-02 01:45:01.000000 dice-3.1.2/dice/__main__.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1715 2021-01-02 01:45:01.000000 dice-3.1.2/dice/command.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      200 2021-01-02 01:45:01.000000 dice-3.1.2/dice/constants.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)    24024 2021-04-07 21:55:21.000000 dice-3.1.2/dice/elements.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)      980 2021-04-07 21:55:21.000000 dice-3.1.2/dice/exceptions.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     6187 2021-01-02 01:45:01.000000 dice-3.1.2/dice/grammar.py
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-04-07 22:01:43.427116 dice-3.1.2/dice/tests/
--rw-r--r--   0 caleb     (1000) caleb     (1000)       33 2021-01-02 01:45:01.000000 dice-3.1.2/dice/tests/__init__.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1025 2021-01-02 01:45:01.000000 dice-3.1.2/dice/tests/test_command.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     6149 2021-04-07 21:55:21.000000 dice-3.1.2/dice/tests/test_elements.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     8010 2021-01-02 01:45:01.000000 dice-3.1.2/dice/tests/test_grammar.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     3309 2021-01-02 01:45:01.000000 dice-3.1.2/dice/tests/test_utilities.py
--rw-r--r--   0 caleb     (1000) caleb     (1000)     4426 2021-01-02 01:45:01.000000 dice-3.1.2/dice/utilities.py
-drwxr-xr-x   0 caleb     (1000) caleb     (1000)        0 2021-04-07 22:01:43.423783 dice-3.1.2/dice.egg-info/
--rw-r--r--   0 caleb     (1000) caleb     (1000)    11238 2021-04-07 22:01:43.000000 dice-3.1.2/dice.egg-info/PKG-INFO
--rw-r--r--   0 caleb     (1000) caleb     (1000)      471 2021-04-07 22:01:43.000000 dice-3.1.2/dice.egg-info/SOURCES.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)        1 2021-04-07 22:01:43.000000 dice-3.1.2/dice.egg-info/dependency_links.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)       69 2021-04-07 22:01:43.000000 dice-3.1.2/dice.egg-info/entry_points.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)       31 2021-04-07 22:01:43.000000 dice-3.1.2/dice.egg-info/requires.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)        5 2021-04-07 22:01:43.000000 dice-3.1.2/dice.egg-info/top_level.txt
--rw-r--r--   0 caleb     (1000) caleb     (1000)       67 2021-04-07 22:01:43.427116 dice-3.1.2/setup.cfg
--rw-r--r--   0 caleb     (1000) caleb     (1000)     1540 2021-04-07 21:55:21.000000 dice-3.1.2/setup.py
+-rw-r--r--   0        0        0      466 2023-05-18 15:52:12.546179 dice-4.0.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0       97 2023-05-18 14:53:20.666178 dice-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1104 2023-05-18 15:16:06.316179 dice-4.0.0/LICENSE.md
+-rw-r--r--   0        0        0     7735 2023-05-18 16:07:45.716178 dice-4.0.0/README.md
+-rw-r--r--   0        0        0     1662 2023-05-18 15:52:56.456179 dice-4.0.0/dice/__init__.py
+-rw-r--r--   0        0        0       95 2023-05-18 15:35:39.216179 dice-4.0.0/dice/__main__.py
+-rw-r--r--   0        0        0     2310 2023-05-18 17:15:16.116179 dice-4.0.0/dice/command.py
+-rw-r--r--   0        0        0      188 2023-05-18 15:48:56.816178 dice-4.0.0/dice/constants.py
+-rw-r--r--   0        0        0    23877 2023-05-18 15:49:16.886178 dice-4.0.0/dice/elements.py
+-rw-r--r--   0        0        0      980 2023-05-18 15:48:56.836178 dice-4.0.0/dice/exceptions.py
+-rw-r--r--   0        0        0     6324 2023-05-18 15:36:07.876179 dice-4.0.0/dice/grammar.py
+-rw-r--r--   0        0        0       33 2023-05-18 14:50:55.646179 dice-4.0.0/dice/tests/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-18 15:35:12.836179 dice-4.0.0/dice/tests/test_command.py
+-rw-r--r--   0        0        0     5999 2023-05-18 15:48:56.936178 dice-4.0.0/dice/tests/test_elements.py
+-rw-r--r--   0        0        0     7870 2023-05-18 15:37:09.336178 dice-4.0.0/dice/tests/test_grammar.py
+-rw-r--r--   0        0        0     2644 2023-05-18 15:37:14.526178 dice-4.0.0/dice/tests/test_utilities.py
+-rw-r--r--   0        0        0     3234 2023-05-18 15:48:56.896178 dice-4.0.0/dice/utilities.py
+-rw-r--r--   0        0        0     1537 2023-05-18 16:07:18.656178 dice-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      290 2023-05-18 15:48:42.556178 dice-4.0.0/tox.ini
+-rw-r--r--   0        0        0     9087 1970-01-01 00:00:00.000000 dice-4.0.0/PKG-INFO
```

### Comparing `dice-3.1.2/README.rst` & `dice-4.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,192 +1,172 @@
-====
-dice
-====
+# dice
 
-.. image:: https://img.shields.io/pypi/v/dice.svg
-    :target: https://pypi.python.org/pypi/dice
-    :alt: Latest PyPI version
+A Python library and command line tool for parsing and evaluating dice notation.
 
-.. image:: https://img.shields.io/travis/borntyping/python-dice.svg
-    :target: https://travis-ci.org/borntyping/python-dice
-    :alt: Travis-CI build status
+_I consider this library "finished", and don't expect to add any more features to it. Bug and security fixes may still be released, especially if you find any bugs after all this time. If you're interested in other libraries in this space, [dyce] has [a great comparison table][comparison-to-alternatives] of Python dice rolling libraries._
 
-.. image:: https://coveralls.io/repos/github/borntyping/python-dice/badge.svg
-    :target: https://coveralls.io/github/borntyping/python-dice
-    :alt: Coveralls coverage score
+[dyce]: https://posita.github.io/dyce/latest/
+[comparison-to-alternatives]: https://posita.github.io/dyce/0.6/#comparison-to-alternatives
 
+## Quickstart
 
-A library and command line tool for parsing and evaluating dice notation.
+### Command-line
 
-Usage
-=====
+```shell
+$ roll 3d6
+```
 
-From the command line, as a pip-installed entry point::
+The command line arguments are as follows:
 
-    $ roll 3d6
+* `-m` `--min` Make all rolls the lowest possible result
+* `-M` `--max` Make all rolls the highest possible result
+* `-h` `--help` Show this help text
+* `-v` `--verbose` Show additional output
+* `-V` `--version` Show the package version
 
-or as a module::
+If your expression begins with a dash (`-`), then put a double dash (`--`)
+before it to prevent the parser from trying to process it as a command option.
+Example: `roll -- -10d6`. Alternatively, use parenthesis: `roll (-10d6)`.
 
-    $ python -m dice 3d6
+### Python API
 
-The command line arguments are as follows::
+Invoking from python:
 
-    -m --min        Make all rolls the lowest possible result
-    -M --max        Make all rolls the highest possible result
-    -h --help       Show this help text
-    -v --verbose    Show additional output
-    -V --version    Show the package version
+```python
+import dice
+dice.roll('3d6')
+```
 
-If your expression begins with a dash (``-``), then put a double dash (``--``)
-before it to prevent docopt from trying to process it as a command option.
-Example: ``roll -- -10d6``. Alternatively, use parenthesis: ``roll (-10d6)``.
+This returns an `Element` which is the result of the roll, which can be a
+`list`, `int`, or subclass thereof, depending on the top-level operator.
 
-Invoking from python::
+## Usage
 
-    import dice
-    dice.roll('3d6')
+### Installation
 
-This returns an ``Element`` which is the result of the roll, which can be a
-``list``, ``int``, or subclass thereof, depending on the top-level operator.
+This library is available as `dice` on PyPI. Install it with your Python
+package or dependency manager of choice — if you're installing it as a
+command-line tool, I recommend [pipx].
 
-Notation
-========
+A recent version of Python 3 (3.8 or above) is required. You can probably run
+it or easily adapt it for older versions of Python, but I don't support any
+end-of-life Python versions. Beyond that, the only dependency is the `pyparsing` library.
+
+[pipx]: https://pypa.github.io/pipx/
+
+### Notation
 
 The expression works like a simple equation parser with some extra operators.
 
 *The following operators are listed in order of precedence. Parentheses may
 be used to force an alternate order of evaluation.*
 
-The dice (``[N]dS``) operator takes an amount (N) and a number of sides (S), and
-returns a list of N random numbers between 1 and S. For example: ``4d6`` may
-return ``[6, 3, 2, 4]``. Usin a ``%`` as the second operand is shorthand for 
-rolling a d100, and a using ``f`` is shorthand for ±1 fudge dice.
+The dice (`[N]dS`) operator takes an amount (N) and a number of sides (S), and
+returns a list of N random numbers between 1 and S. For example: `4d6` may
+return `[6, 3, 2, 4]`. Using a `%` as the second operand is shorthand for 
+rolling a d100, and a using `f` is shorthand for ±1 fudge dice.
 
-The fudge dice (``[N]uS``) operator is interchangable with the dice operator,
-but makes the dice's range from -S to S instead of 1 to S. This includes 0.
+The fudge dice (`[N]uS`) operator is interchangeable with the dice operator,
+but makes the dice range from -S to S instead of 1 to S. This includes 0.
 
-A wild dice (``[N]wS``) roll is special. The last roll in this set is called the
+A wild dice (`[N]wS`) roll is special. The last roll in this set is called the
 "wild die". If this die's roll is the maximum value, the second-highest roll
 in the set is set to the maximum value. If its roll is the minimum, then
 both it and the highest roll in the set aer set to zero. Then another die is
 rolled. If this roll is the minimum value again, then ALL die are set to zero.
 If a single-sided wild die is rolled, the roll behaves like a normal one.
 
 If N is not specified, it is assumed you want to roll a single die.
-``d6`` is equivalent to ``1d6``.
+`d6` is equivalent to `1d6`.
 
-Rolls can be exploded with the ``x`` operator, which adds an additional dice
+Rolls can be exploded with the `x` operator, which adds additional dice
 to the set for each roll above a given threshold. If a threshold isn't given,
 it defaults to the maximum possible roll. If the extra dice exceed this
 threshold, they "explode" again! Safeguards are in place to prevent this from
 crashing the parser with infinite explosions.
 
-You can make the parser reroll dice below a certain threshold with the ``r``
-and ``rr`` operators. The single ``r`` variety allows the new roll to be below
+You can make the parser re-roll dice below a certain threshold with the `r`
+and `rr` operators. The single `r` variety allows the new roll to be below
 the threshold, whereas the double variety's roll *changes* the roll range to
 have a minimum of the threshold. The threshold defaults to the minimum roll.
 
 The highest, middle or lowest rolls or list entries can be selected with
-(``^`` or ``h``), (``m`` or ``o``), or (``v`` or ``l``) respectively.
-``6d6^3`` will keep the highest 3 rolls, whereas ``6d6v3`` will select
+(`^` or `h`), (`m` or `o`), or (`v` or `l`) respectively.
+`6d6^3` will keep the highest 3 rolls, whereas `6d6v3` will select
 the lowest 3 rolls. If a number isn't specified, it defaults to keeping all
 but one for highest and lowest, and all but two for the middle. If a negative
 value is given as the operand for any of these operators, this operation will
-drop that many elements from the result. For example, ``6d6^-2`` will drop the
+drop that many elements from the result. For example, `6d6^-2` will drop the
 two lowest values from the set, leaving the 4 highest. Zero has no effect.
 
-A variant of the explode operator is the ``a`` ("again") operator. Instead of
+A variant of the "explode" operator is the `a` ("again") operator. Instead of
 re-rolling values equal to or greater than the threshold (or max value), this
 operator doubles values *equal* to the provided threshold (or max value). When
 no right-side operand is specified, the left side must be a dice expression.
 
 There are two operators for taking a set of rolls or numbers and counting the
 number of elements at or above a certain threshold, or "successes". Both
-require a right-hand operand for the threshold. The first, ``e``, only counts
-successes. The second, ``f``, counts successes minus failures, which are when
+require a right-hand operand for the threshold. The first, `e`, only counts
+successes. The second, `f`, counts successes minus failures, which are when
 a roll is the minimum possible value for the die element, or 1 for lists.
 
-A list or set of rolls can be turned into an integer with the total (``t``)
-operator. ``6d1t`` will return ``6`` instead of ``[1, 1, 1, 1, 1, 1]``.
+A list or set of rolls can be turned into an integer with the total (`t`)
+operator. `6d1t` will return `6` instead of `[1, 1, 1, 1, 1, 1]`.
 Applying integer operations to a list of rolls will total them automatically.
 
-A set of dice rolls can be sorted with the sort (``s``) operator. ``4d6s``
+A set of dice rolls can be sorted with the sort (`s`) operator. `4d6s`
 will not change the return value, but the dice will be sorted from lowest to
 highest.
 
-The ``+-`` operator is a special prefix for sets of rolls and lists. It
-negates odd roles within a list. Example: ``[1, 2, 3]`` -> ``[-1, 2, -3]``.
-There is also a negate (``-``) operator, which works on either single
-elements, sets or rolls, or lists. There is also an identity ``+`` operator.
+The `+-` operator is a special prefix for sets of rolls and lists. It
+negates odd roles within a list. Example: `[1, 2, 3]` -> `[-1, 2, -3]`.
+There is also a negate (`-`) operator, which works on either single
+elements, sets or rolls, or lists. There is also an identity `+` operator.
 
 Values can be added or subtracted from each element of a list or set of rolls
-with the pointwise add (``.+``) and subtract (``.-``) operators. For example:
-``4d1 .+ 3`` will return ``[4, 4, 4, 4]``.
+with the point-wise add (`.+`) and subtract (`.-`) operators. For example:
+`4d1 .+ 3` will return `[4, 4, 4, 4]`.
 
-Basic integer operations are also available: ``(16 / 8 * 4 - 2 + 1) % 4 -> 3``.
+Basic integer operations are also available: `(16 / 8 * 4 - 2 + 1) % 4 -> 3`.
 
 
 Finally, there are two operators for building and extending lists. To build a
-list, use a comma to seperate elements. If any comma-seperated item isn't a
+list, use a comma to separate elements. If any comma-seperated item isn't a
 scalar (e.g. a  roll), it is flattened into one by taking its total. The
-extend operator (``|``) is used to merge two lists into one, or append single
+"extend" operator (`|`) is used to merge two lists into one, or append single
 elements to the beginning or end of a list.
 
-API
-===
+### Python API
 
-The calls to ``dice.roll()`` above may be replaced with ``dice.roll_min()`` or
-``dice.roll_max()`` to force ALL rolls to their highest or lowest values
-respectively. This might be useful to see what the minumum and maximum
+The calls to `dice.roll()` above may be replaced with `dice.roll_min()` or
+`dice.roll_max()` to force ALL rolls to their highest or lowest values
+respectively. This might be useful to see what the minimum and maximum
 possible values for a given expression are. Beware that this causes wild dice
 rolls to act like normal ones, and rolls performed as explosions are not
 forced high or low.
 
-The ``roll()`` function and variants take a boolean ``raw`` parameter which
+The `roll()` function and variants take a boolean `raw` parameter which
 makes the library return the element instead of the result. Note that the 
-``evaluate_cached`` method is called as part of ``roll()``, which populates
-``element.result``. Calling ``element.evaluate()`` will not reset this value.
+`evaluate_cached` method is called as part of `roll()`, which populates
+`element.result`. Calling `element.evaluate()` will not reset this value.
 
 To display a verbose breakdown of the element tree, the
-``dice.utilities.verbose_print(element)`` function is available.
-If ``element.result`` has not yet been populated, the function calls
-``evaluate_cached()`` first. Keep this in mind if you want to print the result
-of an evaluation with custom arguments. ``verbose_print()`` returns a ``str``.
-
-Most evaluation errors will raise ``DiceError`` or ``DiceFatalError``, both of
-which are subclasses of ``DiceBaseError``. These exceptions have a method
-named ``pretty_print``, which will output a string indicating where the error
+`dice.utilities.verbose_print(element)` function is available.
+If `element.result` has not yet been populated, the function calls
+`evaluate_cached()` first. Keep this in mind if you want to print the result
+of an evaluation with custom arguments. `verbose_print()` returns a `str`.
+
+Most evaluation errors will raise `DiceError` or `DiceFatalError`, both of
+which are subclasses of `DiceBaseError`. These exceptions have a method
+named `pretty_print`, which will output a string indicating where the error
 happened::
 
-    >>> try:
-    ...   dice.roll('1/0')
-    ... except dice.DiceBaseException as e:
-    ...   print(e.pretty_print())
-    ...
-    1/0
-      ^ Division by zero
-    >>>
-
-Licence
-=======
-
-The MIT License (MIT)
-
-Copyright (c) 2013 Sam Clements, 2017 Caleb Johnson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
+```python-repl
+>>> try:
+...   dice.roll('1/0')
+... except dice.DiceBaseException as e:
+...   print(e.pretty_print())
+...
+1/0
+  ^ Division by zero
+>>>
+```
```

### Comparing `dice-3.1.2/dice/__init__.py` & `dice-4.0.0/dice/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """A library for parsing and evaluating dice notation."""
 
-from __future__ import absolute_import, print_function, unicode_literals
-
 from pyparsing import ParseBaseException
 
 import dice.elements
 import dice.grammar
 import dice.utilities
 from dice.constants import DiceExtreme
 from dice.exceptions import DiceBaseException, DiceException, DiceFatalException
@@ -19,16 +17,16 @@
     "utilities",
     "command",
     "DiceBaseException",
     "DiceException",
     "DiceFatalException",
     "DiceExtreme",
 ]
-__author__ = "Sam Clements <sam@borntyping.co.uk>, " "Caleb Johnson <me@calebj.io>"
-__version__ = "3.1.2"
+__author__ = "Sam Clements <sam@borntyping.co.uk>, Caleb Johnson <me@calebj.io>"
+__version__ = "4.0.0"
 
 
 def roll(string, **kwargs):
     """Parses and evaluates a dice expression"""
     return _roll(string, **kwargs)
```

### Comparing `dice-3.1.2/dice/elements.py` & `dice-4.0.0/dice/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Objects used in the evaluation of the parse tree"""
 
-from __future__ import absolute_import, print_function, unicode_literals
-
 import random
 import operator
 from pyparsing import ParseFatalException
 from copy import copy
 
 from dice.constants import MAX_EXPLOSIONS, MAX_ROLL_DICE, DiceExtreme
 from dice.exceptions import DiceFatalException
 from dice.utilities import classname, add_even_sub_odd, dice_switch
 
 
-class Element(object):
+class Element:
     @classmethod
     def parse(cls, string, location, tokens):
         try:
             return cls(*tokens).set_parse_attributes(string, location, tokens)
         # The following only matters on python2 platforms, so is marked nocover
         except ArithmeticError as e:  # nocover
             exc = DiceFatalException(string, location, e.args[0])  # nocover
@@ -193,15 +191,15 @@
             elif self.force_extreme is DiceExtreme.EXTREME_MIN:
                 rolled = [min_value] * amount
             elif self.force_extreme is DiceExtreme.EXTREME_MAX:
                 rolled = [max_value] * amount
             else:
                 rolled = self.do_roll(**kwargs)
 
-        super(Roll, self).__init__(rolled)
+        super().__init__(rolled)
 
     def copy(self):
         return type(self)(
             self.random_element, rolled=self, force_extreme=self.force_extreme
         )
 
     def __repr__(self):
@@ -241,15 +239,15 @@
         return rolls
 
 
 class ExplodedRoll(Roll):
     """Represents an exploded roll"""
 
     def __init__(self, original, rolled, **kwargs):
-        super(ExplodedRoll, self).__init__(original, rolled=rolled, **kwargs)
+        super().__init__(original, rolled=rolled, **kwargs)
 
 
 class RandomElement(Element):
     """Represents a set of elements with a random numerical result"""
 
     DICE_MAP = {}
     SEPARATOR = None
@@ -333,15 +331,15 @@
 @RandomElement.register_dice
 class Dice(RandomElement):
     """A group of dice, all with the same number of sides"""
 
     SEPARATOR = "d"
 
     def __init__(self, amount, max_value, min_value=1):
-        super(Dice, self).__init__(amount, min_value, max_value)
+        super().__init__(amount, min_value, max_value)
         self.original_operands = (amount, max_value)
 
     @property
     def sides(self):
         return self.max_value
 
     def __repr__(self):
@@ -367,15 +365,15 @@
 @RandomElement.register_dice
 class FudgeDice(Dice):
     """A group of dice whose sides range from -x to x, including 0"""
 
     SEPARATOR = "u"
 
     def __init__(self, amount, value):
-        super(FudgeDice, self).__init__(amount, value, -value)
+        super().__init__(amount, value, -value)
 
     def __repr__(self):
         p = "{0!r}, {1!r}".format(self.amount, self.max_value)
 
         if self.min_value != -self.max_value:
             p += ", {0!r}".format(self.min_value)
 
@@ -549,15 +547,14 @@
                 result -= 1
 
         return result
 
 
 class Again(RHSIntegerOperator):
     def function(self, lhs, rhs=None):
-
         if not isinstance(lhs, IntegerList):
             lhs = IntegerList([lhs])
 
         if rhs is None:
             if not isinstance(lhs, Roll):
                 raise self.fatal("%s is not a random element" % lhs)
 
@@ -775,15 +772,15 @@
 
 class Negate(Operator):
     def __new__(cls, x):
         if isinstance(x, int):
             # Passthrough to prevent Negate() clutter
             return Integer(-x)
 
-        return super(Negate, cls).__new__(cls)
+        return super().__new__(cls)
 
     def function(self, operand):
         operand = IntegerList(operand)
 
         for i, x in enumerate(operand):
             operand[i] = -x
```

### Comparing `dice-3.1.2/dice/exceptions.py` & `dice-4.0.0/dice/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     @classmethod
     def from_other(cls, other):
         if isinstance(other, ParseException):
             return DiceException(*other.args)
         elif isinstance(other, ParseFatalException):
             return DiceFatalException(*other.args)
         raise NotImplementedError(
-            'DiceBaseException can only wrap ParseException or ParseFatalException'
+            "DiceBaseException can only wrap ParseException or ParseFatalException"
         )
 
     def pretty_print(self):
         string, location, description = self.args
         lines = string.split("\n")
 
         if len(description) < (self.col - 1):
```

### Comparing `dice-3.1.2/dice/grammar.py` & `dice-4.0.0/dice/grammar.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 Dice notation grammar
 
 PyParsing is patched to make it easier to work with, by removing features
 that get in the way of development and debugging. See the dice.utilities
 module for more information.
 """
 
-from __future__ import absolute_import, print_function, unicode_literals
+import warnings
 
 from pyparsing import (
     CaselessLiteral,
     Forward,
     Literal,
     OneOrMore,
     Or,
+    ParserElement,
     StringStart,
     StringEnd,
     Suppress,
     Word,
     nums,
     opAssoc,
 )
@@ -46,17 +47,20 @@
     SuccessFail,
     ArrayAdd,
     ArraySub,
     RandomElement,
     Again,
 )
 
-from dice.utilities import patch_pyparsing, wrap_string
+from dice.utilities import wrap_string
 
-patch_pyparsing()
+# Enables pyparsing's packrat parsing, which is much faster
+# for the type of parsing being done in this library.
+warnings.warn("Enabled pyparsing packrat parsing", ImportWarning)
+ParserElement.enablePackrat()
 
 
 def operatorPrecedence(base, operators):
     """
     This re-implements pyparsing's operatorPrecedence function.
 
     It gets rid of a few annoying bugs, like always putting operators inside
```

### Comparing `dice-3.1.2/dice/tests/test_command.py` & `dice-4.0.0/dice/tests/test_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-
 from dice import roll, roll_min, roll_max
 from dice.command import main
 from itertools import product
 from pytest import raises
 
 
 def test_roll():
```

### Comparing `dice-3.1.2/dice/tests/test_elements.py` & `dice-4.0.0/dice/tests/test_elements.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-
 from dice.constants import DiceExtreme
 from dice.exceptions import DiceException, DiceFatalException
 import pickle
 from pytest import raises
 import random
 
 from dice.elements import (
@@ -17,15 +15,15 @@
     Element,
     RandomElement,
     WildDice,
 )
 from dice import roll, roll_min, roll_max
 
 
-class TestElements(object):
+class TestElements:
     def test_integer(self):
         assert isinstance(Integer(1), int)
 
     def test_dice_construct(self):
         d = Dice(2, 6)
         assert d.amount == 2 and d.amount == 2 and d.sides == d.max_value == 6
 
@@ -106,15 +104,15 @@
 
     def test_wild_critfail(self):
         while True:
             if WildRoll.roll(3, 1, 2) == [0, 0, 0]:
                 break
 
 
-class TestErrors(object):
+class TestErrors:
     def test_toomanydice(self):
         with raises(DiceFatalException):
             roll("%id6" % (MAX_ROLL_DICE + 1))
 
         with raises(DiceFatalException):
             roll("7d6", max_dice=6)
 
@@ -135,20 +133,20 @@
         with raises(DiceFatalException):
             rolled = roll("6d6")
             rolled.do_roll_single(4, 3)
 
     def test_invalid_wrap(self):
         with raises(NotImplementedError):
             try:
-                raise RuntimeError('blah')
+                raise RuntimeError("blah")
             except Exception as e:
                 raise DiceException.from_other(e)
 
 
-class TestEvaluate(object):
+class TestEvaluate:
     def test_cache(self):
         """Test that evaluation returns the same result on successive runs"""
         roll("6d(6d6)t")
         ast = Total(Dice(6, Dice(6, 6)))
         evals = [ast.evaluate_cached() for i in range(100)]
         assert len(set(evals)) == 1
         assert ast.evaluate_cached() is ast.evaluate_cached()
@@ -163,15 +161,15 @@
         """Test that binary operators function properly when repeated"""
         assert roll("1d1+1d1+1d1") == 3
         assert roll("1d1-1d1-1d1") == -1
         assert roll("1d1*1d1*1d1") == 1
         assert roll("1d1/1d1/1d1") == 1
 
 
-class TestRegisterDice(object):
+class TestRegisterDice:
     def test_reregister(self):
         class FooDice(RandomElement):
             SEPARATOR = "d"
 
         with raises(RuntimeError):
             RandomElement.register_dice(FooDice)
 
@@ -186,31 +184,23 @@
         class BazDice(Element):
             pass
 
         with raises(TypeError):
             RandomElement.register_dice(BazDice)
 
 
-class TestSystemRandom(object):
+class TestSystemRandom:
     sysrandom = random.SystemRandom()
 
     # lowest, middle and highest operators use shuffle()
     def test_sysrandom_op(self):
         roll("6d6h1", random=self.sysrandom)
 
     def test_sysrandom_roll(self):
         roll("6d6", random=self.sysrandom)
 
 
-class TestPickle(object):
-    for expr in [
-        '-d20',
-        '4d6t',
-        '+-(1,2,3)',
-        '2d20h',
-        '4d6h3s',
-        '4dF - 2',
-        '4*d%'
-    ]:
+class TestPickle:
+    for expr in ["-d20", "4d6t", "+-(1,2,3)", "2d20h", "4d6h3s", "4dF - 2", "4*d%"]:
         value = roll(expr, raw=True, single=False)
         pickled = pickle.dumps(value)
         clone = pickle.loads(pickled)
```

### Comparing `dice-3.1.2/dice/tests/test_grammar.py` & `dice-4.0.0/dice/tests/test_grammar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from __future__ import absolute_import, unicode_literals, division
-
 from pyparsing import Word, opAssoc
 from dice.elements import Integer, Roll, WildRoll, ExplodedRoll
 from dice.exceptions import DiceException, DiceFatalException
 from dice import roll, roll_min, roll_max, grammar
 from pytest import raises
 
 
-class TestInteger(object):
+class TestInteger:
     def test_value(self):
         assert roll("1337") == 1337
 
     def test_type(self):
         assert isinstance(roll("1"), int)
         assert isinstance(roll("1"), Integer)
 
 
-class TestDice(object):
+class TestDice:
     def test_dice_value(self):
         assert 0 < int(roll("d6")) <= 6
         assert 0 < int(roll("6d6")) <= 36
 
         assert 0 < int(roll("d%")) <= 100
         assert 0 < int(roll("6d%")) <= 600
 
@@ -57,15 +55,15 @@
             assert 0 < die <= 6
 
     def test_nested_dice(self):
         assert 1 <= roll("d(d6)t") <= 6
         assert -6 <= roll("u(d6)t") <= 6
 
 
-class TestOperators(object):
+class TestOperators:
     def test_add(self):
         assert roll("2 + 2") == 4
 
     def test_sub(self):
         assert roll("2 - 2") == 0
 
     def test_mul(self):
@@ -90,15 +88,15 @@
 
     def test_aeso(self):
         assert roll("+-1") == -1
         assert roll("+-2") == 2
         assert roll("+-(1, 2)") == [-1, 2]
 
 
-class TestVectorOperators(object):
+class TestVectorOperators:
     def test_total(self):
         assert (6 * 1) <= roll("6d6t") <= (6 * 6)
 
     def test_sort(self):
         value = roll("6d6s")
         assert value == sorted(value)
         assert isinstance(value, Roll)
@@ -188,15 +186,15 @@
         rr2 = roll("2d6 | 3d6 | 4d6")
         assert len(rr2) == 9
 
         rr3 = roll("2d6 | 3d6 | 10 | 4d6")
         assert len(rr3) == 10
 
 
-class TestDiceOperators(object):
+class TestDiceOperators:
     def test_reroll(self):
         r = roll("6d6r")
         assert len(r) == 6
 
     def test_force_reroll(self):
         r2 = roll("1000d6rr")
         assert 1 not in r2
@@ -224,15 +222,15 @@
         assert roll("6a6") == [6, 6]
 
     def test_again_vector(self):
         assert roll("(1,2,3)a2") == [1, 2, 2, 3]
         assert roll("(1|1|1)a1") == [1, 1, 1, 1, 1, 1]
 
 
-class TestErrors(object):
+class TestErrors:
     @staticmethod
     def run_test(expr):
         with raises((DiceException, DiceFatalException)):
             roll(expr)
 
     def test_bad_operators(self):
         for expr in ("6d", "1+", "[1,2,3]", "f", "3f", "3x", "6.+6", "7.-7"):
@@ -262,37 +260,37 @@
         self.run_test("1/(0*1)")
 
     def test_again_fail(self):
         self.run_test("(1,2,3)a")
         self.run_test("1a")
 
 
-class TestOperatorPrecedence(object):
+class TestOperatorPrecedence:
     def test_operator_precedence_1(self):
         assert roll("16 / 8 * 4 + 2 - 1") == 9
 
     def test_operator_precedence_2(self):
         assert roll("16 - 8 + 4 * 2 / 1") == 16
 
     def test_operator_precedence_3(self):
         assert roll("10 - 3 + 2") == 9
 
     def test_operator_precedence_4(self):
         assert roll("1 + 2 * 3") == 7
 
 
-class TestExpression(object):
+class TestExpression:
     def test_expression(self):
         assert isinstance(roll("2d6"), Roll)
 
     def test_sub_expression(self):
         assert isinstance(roll("(2d6)d(2d6)"), Roll)
 
 
-class TestBadPrecedence(object):
+class TestBadPrecedence:
     def test_invalid_arity(self):
         with raises(Exception):
             grammar.operatorPrecedence(
                 grammar.integer, [(Word("0"), 3, opAssoc.LEFT, Integer.parse)]
             )
 
     def test_invalid_association(self):
```

### Comparing `dice-3.1.2/dice/tests/test_utilities.py` & `dice-4.0.0/dice/tests/test_utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-
 from pyparsing import Literal, ParseFatalException
 from pytest import raises
 import random
 import string
 
 from dice import roll, utilities
 from dice.utilities import verbose_print
@@ -13,32 +11,15 @@
 def test_enable_pyparsing_packrat_parsing():
     """Test that packrat parsing was enabled"""
     import pyparsing
 
     assert pyparsing.ParserElement._packratEnabled is True
 
 
-def test_disable_pyparsing_arity_trimming():
-    """Test that pyparsing._trim_arity has been replaced"""
-    import pyparsing
-    import dice.utilities
-
-    assert pyparsing._trim_arity is dice.utilities._trim_arity
-
-
-def test_disable_pyparsing_arity_trimming_works():
-    """Tests that arity trimming has been disabled and parse actions with
-    the wrong number of arguments will raise TypeErrors"""
-    for func in [lambda a: None, lambda a, b: None, lambda a, b, c, d: None]:
-        element = Literal("test").setParseAction(func)
-        with raises(TypeError):
-            element.parseString("test")
-
-
-class TestVerbosePrint(object):
+class TestVerbosePrint:
     def _get_vprint(self, expr):
         raw = roll(expr, raw=True)
         evaluated = raw.evaluate_cached()
         vprint = verbose_print(raw)
         return evaluated, vprint
 
     def test_dice_simple(self):
@@ -64,15 +45,15 @@
         assert v.startswith("roll 1d20 -> ")
 
     def test_single_line(self):
         v = self._get_vprint("d6x")[1]
         assert len(v.split("\n")) == 1
 
 
-class TestDiceSwitch(object):
+class TestDiceSwitch:
     def test_separator_map(self):
         for sep, cls in RandomElement.DICE_MAP.items():
             d = utilities.dice_switch(6, 6, sep)
             assert type(d) is cls
 
     def test_percentile(self):
         for sep, cls in RandomElement.DICE_MAP.items():
```

### Comparing `dice-3.1.2/setup.py` & `dice-4.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,48 @@
-#!/usr/bin/python
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
-from __future__ import absolute_import, print_function, unicode_literals
-from setuptools import setup, find_packages
+[project]
+name = "dice"
+version = "4.0.0"
+authors = [
+    { name = "Sam Clements", email = "sam@borntyping.co.uk" },
+    { name = "Caleb Johnson", email = "me@calebj.io" },
+]
+maintainers = [
+    { name = "Sam Clements", email = "sam@borntyping.co.uk" },
+]
+description = "A library for parsing and evaluating dice notation"
+readme = "README.md"
+requires-python = ">=3.7"
+license = { text = "MIT" }
+classifiers = [
+    "Development Status :: 6 - Mature",
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Other Audience",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Games/Entertainment",
+    "Topic :: Games/Entertainment :: Board Games",
+    "Topic :: Games/Entertainment :: Role-Playing",
+    "Topic :: Games/Entertainment :: Multi-User Dungeons (MUD)",
+    "Topic :: Games/Entertainment :: Turn Based Strategy",
+    "Topic :: Utilities",
+]
+keywords = ["dice"]
+dependencies = [
+    "pyparsing>=2.4.1",
+]
+urls = { homepage = "https://github.com/borntyping/python-dice" }
 
-setup(
-    name="dice",
-    version="3.1.2",
-    author="Sam Clements",
-    author_email="sam@borntyping.co.uk",
-    url="https://github.com/borntyping/python-dice",
-    description="A library for parsing and evaluating dice notation",
-    long_description=open("README.rst").read(),
-    license="MIT",
-    packages=find_packages(),
-    install_requires=["docopt>=0.6.1", "pyparsing>=2.4.1"],
-    entry_points={
-        "console_scripts": ["dice = dice.command:main", "roll = dice.command:main"]
-    },
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Console",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Other Audience",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Topic :: Games/Entertainment",
-        "Topic :: Games/Entertainment :: Board Games",
-        "Topic :: Games/Entertainment :: Role-Playing",
-        "Topic :: Games/Entertainment :: Multi-User Dungeons (MUD)",
-        "Topic :: Games/Entertainment :: Turn Based Strategy",
-        "Topic :: Utilities",
-    ],
-)
+[project.scripts]
+dice = "dice.command:main"
+roll = "dice.command:main"
```

