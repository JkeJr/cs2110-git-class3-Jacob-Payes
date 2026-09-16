# CS 2110 Git Class 3

Software Development Tools

Starter repository for practicing branches, pull requests, merging, and merge conflicts. Fork this repository into your own GitHub account before starting.

## Get started

Fork on GitHub, then clone **your fork** from the command line:

```bash
git clone <your-fork-url>
cd cs2110-git-class3
git remote -v
git status
```

`origin` should point to your fork. Open `index.html` in a browser to view the page.

## Workflow cheat sheet

**Do not make assignment changes directly on `main` unless instructed.** Repeat this workflow for each feature:

1. Start from an updated local `main` and create a branch:
   ```bash
   git switch main
   git pull origin main
   git switch -c feature-about
   ```
   Use a new, descriptive branch name for each feature.
2. Make your changes, then review and commit them:
   ```bash
   git status
   git diff
   git add index.html
   git commit -m "Update About Me section"
   ```
   Stage the files you actually changed.
3. Push your branch:
   ```bash
   git push -u origin feature-about
   ```
4. On GitHub, create a pull request **in your fork**, from your feature branch into your fork's `main`. Check the base repository carefully.
5. Review the commits and files changed, then merge the pull request on GitHub.
6. Update local `main`:
   ```bash
   git switch main
   git pull origin main
   ```

## Merge-conflict practice

Leave the following line unchanged until your instructor starts the controlled merge-conflict exercise.

Favorite Git Command: TBD
