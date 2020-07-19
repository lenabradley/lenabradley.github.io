---
layout: post
title: Python and Software Notes 
---

Notes, resources, and links for python and software in general


# Python
* Google's python class https://developers.google.com/edu/python
* PEPs
    * all: https://www.python.org/dev/peps/
    * style guide (old but still mostly good): https://www.python.org/dev/peps/pep-0008/
    * zen of python: https://www.python.org/dev/peps/pep-0020/
* Python Bytes podcast: https://pythonbytes.fm/
* Python testing
    * https://medium.com/@yeraydiazdiaz/what-the-mock-cheatsheet-mocking-in-python-6a71db997832
    * https://medium.com/@bfortuner/python-unit-testing-with-pytest-and-mock-197499c4623c
    * use pytest (instead of unittest)
    * Understand the difference between these concepts:
        * Testing library/package
        * test runner
        * test discovery
        * parameterization
        * fixtures (pytest-specific)
        * snapshot testing
* Tools, Packages, and features: An incomplete listing
    * Some of my favorite python features
        * type hinting (3.5+)
        * dataclasses (3.7+, can use attrs package instead if in an earlier version of python)
        * f-strings (3.6+)
    * Packages I use often and love to use
        * pint
        * pathlib (in standardlib)
        * poetry
        * loguru
    * Packages I use often but do not love
        * pymap3d
        * snapshottest (use this fork NOT the package on PyPI https://github.com/YAtOff/snapshottest)
    * Packages I use often and have mixed feelings about
        * pytest
        * pandas
        * sqlalchemy
    * Packages I use for plotting (ordered by preference)
        * seaborn
        * plotly
        * matplotlib
    * Related tools I use often
        * pyenv
        * docker
    * Things I recommend NOT using
        * pipenv
 
# General Software
* Clean Code by Robert Cecil Martin (easy to read, good place to start, intuitive)
* A philosophy of Software Design by Josh Ousterhout
* 4 Principles of OOP
    * Encapsulation
    * Abstraction
    * Inheritance
    * Polymorphism
* Rules of thumb, words of wisdom
    * One object (class) does one thing
    * Once class per file
    * Avoid inheritance, prefer composition
    * Manage complexity
    * Code should be readable and make sense when you read it (self-documenting)
    * ... but no code is perfectly self-documenting so always include comments
    * Comments should be clear
    * Do not include "TODOs" in finalized code. This should be gone by PR time
    * Do not include "dead code" (commented-out or otherwise unreachable code). This should all be gone by PR time
    * Always include tests, and CI (e.g. Jenkins) for automated building/testing
    * Naming
        * Naming is more important thank you think!
        * The name should reflect the identity, purpose
        * Never use one-letter names
        * Use consistent naming style (e.g. snake_case, vs camelCase, etc)
        * Where there is not already another standard: refer to PEP8
        * Spell out full words in names (e.g. "utilities" instead of "utils")
    * Write clear, verbose, specific error messages
    * Use logging (e.g. loguru package). use it often. use it instead of just printing debug info to screen
* Documentation
    * Always include docstrings that describe the purpose and approach
    * Suggestion: use "google" docstring style (setting in PyCharm)
* Testing
    * https://mtlynch.io/good-developers-bad-tests/
    * "When you write a test, think about the next developer who will see the test break."
* Code reviews
    * Prefer small PRs to Large PRs
    * When designing something big and/or new and/or if you are uncertain: Get eyes on your code early and often
    * When you want feedback: Show people actual code and provide context for the use case. D
        * Preferred: Bitbucket link to the code
        * Backup: Provide a code sample that recreates the issue
    * https://google.github.io/eng-practices/review/reviewer/comments.html
    * Provide code samples
 
