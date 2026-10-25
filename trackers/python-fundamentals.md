# Python Fundamentals Tracker

Last updated: 2026-10-25
Rule: tick [x] only after I confirm it is clear or I solve an exercise myself.
Background: I know Java and basic DSA. Zero Python syntax at the start. Compare with Java wherever possible.

## My setup
- Windows, Python 3.10.9, PyCharm with a .venv virtual environment (Thonny and CMD also work)
- Project folder: E:\SDE-2_preparation\01_python_dsa\01_python_fundamentals (lessons\ and exercises\)
- Earlier practice (phase0 to phase4, 22 files) is copied into lessons\phase0 ... lessons\phase4 (verified: 23 .py files with 01_setup.py)
- Code backup: private GitHub repo sde2-python-dsa (folder 01_python_dsa). Daily: git add . then git commit then git push

## Main resources (real, check links are still live)
- Official Python Tutorial: https://docs.python.org/3/tutorial/
- Python for Everybody (free course and book): https://www.py4e.com
- CS50's Introduction to Programming with Python (free, Harvard): https://cs50.harvard.edu/python/
- Automate the Boring Stuff with Python (free to read online): https://automatetheboringstuff.com

## Topics (what to learn, where to read)
- [x] 01 Setup: editor, run first file, imports. Read: Tutorial ch.2 and ch.6.1 (virtual environment moved to topic 13)
- [x] 02 Variables, types, input/output, f-strings. Done: datatypes, type conversion, input() (always returns a string, wrap in int() for numbers), f-strings with expressions. Read: Tutorial ch.3 and ch.7.1
- [x] 03 Operators, if/else, truthy and falsy. Read: Tutorial ch.4.1
- [x] 04 Loops: for, range, enumerate, zip, while, break/continue/pass, for-else. Read: Tutorial ch.4.2 to 4.5
- [x] 05 Functions: arguments, return, default values, *args, **kwargs, unpacking. Read: Tutorial ch.4.7 to 4.9
- [ ] 06 Lists: slicing, unpacking, comprehensions. Done: basic list methods, slicing (start:stop:step), enumerate. Missing: list comprehension, sort/sorted. Read: Tutorial ch.3.1.3, ch.5.1
- [x] 07 Tuples and sets. Read: Tutorial ch.5.3 to 5.4
- [ ] 08 Dicts (hash table idea, O(1) average). Done: create, get, update, delete. Missing: loop with .items(), .keys(), .values(), dict comprehension. Read: Tutorial ch.5.5
- [ ] 09 Strings and common methods. Done: basics, slicing. Missing: strip, join, split, find, startswith, replace practice. Read: Tutorial ch.3.1.2 and the str methods in the docs
- [ ] 10 Classes and objects (compare with Java). Read: Tutorial ch.9
- [ ] 11 Errors and try/except. Read: Tutorial ch.8
- [ ] 12 Files and input/output. Read: Tutorial ch.7
- [ ] 13 Modules, imports, virtual environments (the .venv already exists in PyCharm; learn how it works here). Read: Tutorial ch.6 and ch.12
- [ ] 14 collections (Counter, defaultdict, deque) and heapq. Read: official docs for `collections` and `heapq`

## Practice files done
- lessons/01_setup.py, exercises/01_setup_ex.py
- lessons/phase0 to phase4: setup and imports, datatypes, operators, strings, list/tuple/dict/set, conditionals, loops, functions, args/kwargs, unpacking (22 files, my earlier work)
- exercises/02_input_fstring.py (input, int(), f-string with age + 1)
- exercises/03_slicing.py (list and string slicing, 6 tasks, all correct)
- Practice functions: is_even, biggest, total, largest (with empty list fix), count_even, count_words, total_by_category

## Known cleanup (small fixes in my own files)
- phase2/04_sets.py: comment says "cherry" in fruits is True, but cherry is never added (it is False)
- phase4/03_unpacking_calls.py: variable named dict hides the built-in dict, and print(**dict) crashes with TypeError
- phase2/02_tuples.py: birth_info.append(...) is not commented out, so the file crashes there
- phase4/02_args_kwargs.py: label says **kwargs packs into a tuple; it packs into a dict. Section also unfinished
- Naming habits: do not reuse built-in names (sum, dict, list); use snake_case for functions; give clear names (numbers, num, words)

## Weekly check-in (neutral, no judgement)
- (date) plan followed? distraction slip? sleep? movement?

## Notes log
- 2026-10-24: Java difference noticed: no main method, no class, no semicolon, no type before variable name
- 2026-10-24: Repo and E: drive folder structure set up. Virtual environment postponed until topic 13
- 2026-10-25: Earlier project reviewed. Topics 01, 03, 04, 05, 07 ticked. Gaps listed in topics 02, 06, 08, 09
- 2026-10-25: Edge case lesson: largest([]) crashed. Fixed with a guard clause (if not numbers: return None)
- 2026-10-25: PyCharm opens and runs with a .venv. Code pushed to private repo sde2-python-dsa (35 objects, no .venv inside)
- 2026-10-25: input() always gives a string. Slicing formula: seq[start:stop:step], stop is not included, negative step goes backwards
- 2026-10-25: Reminder: run git add, commit, push in 01_python_dsa at the end of every session

## Next up
Gap check question 3 of 5: list comprehension (cubes of nums, odd numbers, word lengths) in exercises\04_list_comprehension.py. Then question 4 (dict loops) and 5 (string methods). Then start DSA: Big-O basics
