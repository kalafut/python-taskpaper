# python-taskpaper

python-taskpaper is a Python module for interacting with
[Taskpaper][tp]-formatted documents.

[tp]: https://www.taskpaper.com

## What does it do?

So far?  Not much.   You can open, read and write TaskPaper documents, and
add or remove tags on items within that document, but that's about it.  I'd
like to expand it to be much more powerful, but it depends on when I have
free time.

I will probably change the API in a non-backwards compatible way before 1.0.
User beware.

Look in the `docs` directory for some examples of how I'm using it.

## What does it require?

To use this module, you need Python 2.7 or 3.3+.  Those are the only versions
of Python that I'm interested in testing or writing for.  Standard library
only (for now).

## How do I install it?

Download the `taskpaper.py` script from the root of this repository.
I'll put it on PyPI at some point.

## Why write this?  Why not use the built-in scripting?

Two reasons:

1.  I work with TaskPaper-formatted documents on Windows and Linux (for my day
    job), and the best AppleScript support in the world is utterly useless
    there.  :-(

2.  I prefer Python to AppleScript and JavaScript.

## I hate Python.

Good for you.

There's built-in support for scripting the TaskPaper app with JavaScript or
AppleScript, or Matt Gemmell has written a [Ruby library][gemmell] that you
could use.  (I'd use Matt's library if I actually knew any Ruby.)

[gemmell]: https://github.com/mattgemmell/TaskPaperRuby

## How do I run the tests?

Install `pytest`, `pytest-cov` and `coverage`:

    pip install pytest pytest-cov coverage

then run the tests like so:

    py.test --cov-report term-missing --cov taskpaper.py tests.py

This will run the tests, and show which lines aren't covered by existing tests.
I'm trying to get better at writing tests with good coverage.

## License

The project is licensed under the MIT license.