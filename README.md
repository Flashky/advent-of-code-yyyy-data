# Advent of Code {year} Inputs

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
3. Modify ``README.md``: replace all ``{year}`` occurrences with year in ``yyyy`` format.

## Solutions Repository Setup

This new repository is meant to be used as a [submodule](https://github.blog/2016-02-01-working-with-submodules/) for the main solutions repository:

1. Open [advent-of-code-yyyy](https://github.com/Flashky/advent-of-code-yyyy) template repository.
2. Follow its instructions.

## Almost done...

1. Remove these instructions from ``README.md``.
1. Push the changes and...

**Enjoy your new Advent of Code edition!**

---

Data repository for [advent-of-code-{year}](https://github.com/Flashky/advent-of-code-{year}) solutions repository.

## Update local repository

Use the following command to update the local repo if there are any remote changes:

```bash
git submodule update --recursive --remote
```

## Re-attach local repository

If the local repo becomes detached, execute:

```bash
git checkout master
```

## About

- [Advent of Code](https://adventofcode.com/{year}/about)
