# P2: Portfolio Repository with an Initial Commit

## Aim
To create a simple portfolio webpage, initialise a local Git repository, and save the first version using a Git commit.

## Files
- `index.html` — the structure and content of the portfolio page.
- `style.css` — the styling used by the page.

## Step 1: Create the project and add the webpage files

Create a folder named `P2`. Save the supplied `index.html` and `style.css` files inside it, keeping both files in the same folder.

## Step 2: Open the folder in the terminal

```bash
cd P2
```

## Step 3: Initialise Git and inspect the repository

```bash
git init
git status
```

- `git init` creates a Git repository in the current folder.
- `git status` shows which files are untracked or modified.

## Step 4: Stage and commit the files

```bash
git add index.html style.css README.md
git status
git commit -m "Add initial portfolio page"
```

Staging selects the files to include in the next commit. The commit saves a snapshot of the staged files in the repository history.

## Step 5: Connect to GitHub and push

First create an empty repository on GitHub. Copy its HTTPS URL, then replace the example URL below with your own repository URL.

```bash
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

If a remote named `origin` is already configured, do not add it again. Check it with:

```bash
git remote -v
```

## Expected result
The portfolio files are committed locally. After the push, the same files and the initial commit are visible in the GitHub repository.

## Conclusion
I created a basic portfolio webpage and practised initialising Git, checking repository status, staging files, creating a commit, and pushing the repository to GitHub.
