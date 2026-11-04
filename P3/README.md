# P3: Feature-Branch Git Workflow

## Aim
To practise creating a separate Git branch for a change, committing the change, pushing the branch to GitHub, and merging it through a pull request.

## What is a feature branch?
A feature branch is a separate line of work used to make a change without directly editing the main branch. It helps keep work organised and makes it easier to review changes before merging them.

## Procedure

### Step 1: Check the current branch and working tree

```bash
git status
git branch
```

Make sure there are no unfinished changes that you need to save before switching branches.

### Step 2: Update the main branch

```bash
git switch main
git pull origin main
```

### Step 3: Create and switch to a feature branch

```bash
git switch -c feature/update-about-section
```

The `-c` option creates the branch and switches to it.

### Step 4: Make a small change

Open the portfolio page from P2 and improve the About section. For example, add a sentence describing what you are currently learning. Save the file.

### Step 5: Review, stage, and commit the change

```bash
git status
git diff
git add index.html
git commit -m "Update about section"
```

- `git diff` displays the changes made to tracked files.
- `git add` stages the selected file.
- `git commit` records the staged change.

### Step 6: Push the feature branch

```bash
git push -u origin feature/update-about-section
```

### Step 7: Create a pull request on GitHub

1. Open the repository on GitHub.
2. Select the option to compare or create a pull request for the newly pushed branch.
3. Set the base branch to `main` and the compare branch to `feature/update-about-section`.
4. Review the changes and create the pull request.
5. Merge the pull request after reviewing it.

### Step 8: Update the local main branch

After the pull request is merged:

```bash
git switch main
git pull origin main
git branch -d feature/update-about-section
```

## Workflow summary

`main` → create feature branch → edit file → review changes → commit → push branch → pull request → merge → update main.

## Conclusion
I practised using a feature branch to make an isolated change, reviewing and committing the change, pushing the branch to GitHub, and merging it through a pull request.
