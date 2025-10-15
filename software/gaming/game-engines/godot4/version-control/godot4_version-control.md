# Version Control - Godot 4

You can use git to manage version control with Godot 4.

My recommended approach:

- create folder for the project (herein: `<project-location>`)
- cd `<project-location>`
- git init
- add the following .gitignore file
- !!TODO!! add `.gitignore` link here
- git commit - m “initial commit”
- create an empty repository on origin of choice (example GitHub)
- git remote add origin `<origin-url>`
- git push -u origin main
- Setup branch protection on origin if supported on origin. (Reject pushes directly to main)

Godot 4 provides a .gitignore when you check a certain box or click a certain setting somehwere. !!TODO!! add details about this here.

## Large Files

Game projects usually have at least 1 large file. Adding large files to git can really bloat the size and history of your git project. To resolve this you can use:

- Git Large File System (LFS)
- (optional) local git pre-commit hooks
- (recommended) Continuous Integration (CI) pipeline pre-commit hooks

Here are related bash commands for the precommit hooks. !!TODO!! add details for LFS pre checks.

```bash
#(optional local and recommended CI)
# Requires Python 3
pip instal pre-commit
pre-commit install
```
