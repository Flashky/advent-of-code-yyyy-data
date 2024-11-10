# Advent of Code {year} Data

## How to create a repository from this template repository 

1. Open the main page of [this repository](https://github.com/Flashky/advent-of-code-yyyy-data).
2. Click on **Use this template**.
3. Select **Create a new repository**:
   1. Give a name to the new repository. Example: ``advent-of-code-2022-data``.
   3. Make sure to set as **private**.

### Personal Access Token Setup

In order to the GitHub Actions to be able to perform certain actions, a **Personal Access Token** is needed:

Open **[Account / Settings / Developer Settings / Personal access tokens (classic)](https://github.com/settings/tokens)** and verify if there is any ``PAT_TOKEN`` created.

#### Creating a new token

If there is no ``PAT_TOKEN`` created:

1. Click on **Generate New Token**.
2. Select ``repo`` checkbox.
3. Copy the token.

#### Refreshing an existing token

If there is an existing ``PAT_TOKEN``:

1. Click on it.
2. If the expiration date is due soon, click on **regenerate the token**

#### Adding the token to the repo

1. Open the created repository.
2. Open **Settings / Secrets and variables / Actions** and click on **New repository secret**:
   1. **Name:** ``PAT_TOKEN``
   2. **Secret:** The previously copied token.
  
### Update repository information

1. Go to **Settings / Actions / General**.
2. Under **Workflow permissions**:
   1. Enable **Read and write permissions**.
   2. Enable **Allow GitHub Actions to create and approve pull requests**.
3. Go to **Actions** and open the **Update year** workflow:
   1. Click on **Run workflow**.
   2. Type the year in ``yyyy`` format and click on **Run workflow**.

After the workflow has ended a Pull Request will be created:
1. Open the [pull request](https://github.com/Flashky/advent-of-code-{year}/pull/1).
2. Verify everything is right and then **merge** it.
   
After the PR is merged the repository will have its description and topics updated. Also, all ``README.md`` and ``pom.xml`` will be updated with current year value. The PR can be declined and workflow can be executed again if there was any problem that needed a fix.

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
