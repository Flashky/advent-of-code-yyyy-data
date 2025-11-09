# 💾 Advent of Code {year} Data

## ⚙️ Setup Guide

This guide details the steps to quickly set up your private data repository for the current Advent of Code year.

---

### 🚀 1. New Repository Creation

1.  Open the main page of [this template repository](https://github.com/Flashky/advent-of-code-yyyy-data).
2.  Click **Use this template** and then **Create a new repository**.
3.  Set the repository name (e.g., `advent-of-code-202X-data`).
4.  **Crucially:** Ensure you set the repository visibility to **private**.

### 🔑 2. Token and Secret Configuration

A Personal Access Token (`PAT_TOKEN`) with `repo` scope is required for GitHub Actions to update the repository information automatically.

1.  **Verify/Create the PAT:**
    * Go to **[Personal access tokens (classic)](https://github.com/settings/tokens)**.
    * If you don't have a token named `PAT_TOKEN` (or similar), click **Generate New Token**, select the `repo` scope, and **copy the generated token**.
    * If an existing `PAT_TOKEN` is close to expiring, click on it, select **regenerate the token**, and **copy the new value**.
2.  **Add the PAT to the new repository:**
    * Go to **Settings / Secrets and variables / Actions**.
    * Create a new repository secret: **Name:** `PAT_TOKEN`, **Secret:** *\[Your Token]*

### 📅 3. Year Update and Permissions

This step updates the year in the repository name, description, and files.

1.  **Configure Workflow Permissions:**
    * Go to **Settings / Actions / General**.
    * Under **Workflow permissions**, enable:
        * **Read and write permissions**.
        * **Allow GitHub Actions to create and approve pull requests**.
2.  **Run "Update year" Workflow:**
    * Go to the **Actions** tab and open the **Update year** workflow.
    * Click **Run workflow**, type the **year** in `yyyy` format (e.g., `2025`), and **Run workflow**.
3.  **Merge the Pull Request:**
    * Once the workflow finishes, a Pull Request will be created.
    * **Open it**, verify the year changes are correct, and **merge** it.

> After merging, the repository will be correctly configured for the current year.

### 🔗 4. Solutions Repository Setup

This repository is designed to be used as a **submodule** for your main solutions repository:

1.  Open the [advent-of-code-yyyy](https://github.com/Flashky/advent-of-code-yyyy) template repository.
2.  Follow **its instructions** in the "Data Repository Setup" section to link this private repository as a submodule.

### ✅ 5. Final Steps

1. Remove all these setup instructions from the README.md.
2. Commit and push the changes.

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
