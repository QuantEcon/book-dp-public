# Julia code for *Dynamic Programming, Volume 1*

This directory contains the Julia source files for the figures and
examples in the book.

## Running the scripts

Each script is self-contained and writes any generated figures to
`../figures/` (i.e. `code/figures/` from the repository root).

**Important:** the scripts assume they are run from this directory
(`code/jl/`). For example:

    cd code/jl
    julia finite_opt_saving_2.jl

Running from elsewhere (e.g. the repo root) will cause `savefig` to
fail or write figures to the wrong place, because the `../figures/`
paths are resolved relative to the working directory.
