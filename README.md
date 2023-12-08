# Advent of Code {year} - Inputs

## How to create a repository from this template repository 

1. Open the main page of [this repository](https://github.com/Flashky/advent-of-code-yyyy-data).
2. Click on **Use this template**.
3. Select **Create a new repository**:
   1. Give a name to the new repository. Example: ``advent-of-code-2022-data``.
   2. Add a description to the new repository. Example: ``Advent of Code 2022 - Inputs``.
   3. Make sure to set as **private**.

## Repository Setup

1. Open the created repository.
2. Click on settings next to **About** and add the following tags (using the corresponding year):
    1. ``advent-of-code``
    2. ``advent-of-code-data``
    3. ``advent-of-code-yyyy-data``

## Solutions Repository Setup

This new repository is meant to be used as a [submodule](https://github.blog/2016-02-01-working-with-submodules/) for the main solutions repository:

1. Create the solutions repository using [advent-of-code-yyyy](https://github.com/Flashky/advent-of-code-yyyy) template repository.
2. Clone the created solutions repository.
3. Open ``src/test/resources`` folder.
4. Execute: ``git submodule add https://github.com/Flashky/advent-of-code-{year}-data.git inputs``

## About

- [Advent of Code](https://adventofcode.com/{year}/about)
