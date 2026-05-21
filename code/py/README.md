# Python code for *Dynamic Programming, Volume 1*

This directory contains the Python source files for the figures and
examples in the book.

## Running the scripts

Each script is self-contained and writes any generated figures to
`../figures_py/` (i.e. `code/figures_py/` from the repository root).

**Important:** the scripts assume they are run from this directory
(`code/py/`). For example:

    cd code/py
    python finite_opt_saving_2.py

Running from elsewhere (e.g. the repo root) will cause `savefig` to
fail or write figures to the wrong place, because the `../figures_py/`
paths are resolved relative to the working directory.
