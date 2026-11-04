# P4: GitHub README and Version Tags

## Aim
To prepare a clear README file for a GitHub repository and use Git tags to identify a version of the project.

## Part A: Create a README file

A README is usually the first file people see when they open a repository. It explains the purpose of the project, its files, and how to view or use it.

Create a file named `README.md` in the root of the repository. A simple example is:

```markdown
# Student Portfolio

A basic portfolio webpage created while practising HTML, CSS, and Git.

## Files
- index.html — contains the webpage structure.
- style.css — contains the page styling.

## How to view
Open index.html in a web browser.

## Topics practised
- HTML page structure
- CSS styling
- Git version control
```

Save the README file. Markdown headings use `#`, and bullet points use hyphens.

## Part B: Stage and commit the README

```bash
git status
git add README.md
git commit -m "Add project README"
```

If the README is already committed and you make further edits, stage and commit those updates in the same way.

## Part C: Create a version tag

An annotated tag stores a version label and a message.

```bash
git tag -a v1.0.0 -m "First complete lab version"
```

## Part D: Push the tag to GitHub

```bash
git push origin v1.0.0
```

To push all local tags instead:

```bash
git push origin --tags
```

## Part E: View and inspect tags

```bash
# List all tags
git tag

# Display information about a tag
git show v1.0.0
```

## Version number explanation

For this practical, `v1.0.0` marks the first prepared version. A version number commonly follows the pattern `MAJOR.MINOR.PATCH`:

- **MAJOR** — a significant change that may not be compatible with an earlier version.
- **MINOR** — a new feature that keeps existing functionality compatible.
- **PATCH** — a small fix or correction.

## Expected result
The repository has a useful README file, and the version tag `v1.0.0` can be seen in the local Git tag list and on GitHub after it is pushed.

## Conclusion
I practised writing a repository README, committing it with Git, creating an annotated version tag, and pushing and inspecting tags.
