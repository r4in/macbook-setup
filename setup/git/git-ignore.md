# Git Ignore

This tells git which files or folders not to track or upload to your repo.&#x20;

Create the file `~/.gitignore` as shown below, so you don’t track files that are almost always ignored in Git repositories. Why do we need a global one? So you don’t have to repeat the same “junk ignores” in every project.

```
touch ~/.gitignore
```

Open the `.gitignore` file using your favorite text editor and add the following:

```
# macOS
.DS_Store
._*

# Windows (optional but harmless)
Thumbs.db

# Editors
.vscode/
.idea/

# Logs
*.log
```

The tell git to use it:

```
git config --global core.excludesfile ~/.gitignore
```

