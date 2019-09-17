# Git Ignore

Create the file `~/.gitignore`as shown below to not track files that are almost always ignored in all Git repositories.

```text
touch ~/.gitignore
```

Open the `.gitignore` file using your favourite text editor and add these below:

```text
# Folder view configuration files
.DS_Store
Desktop.ini

# Thumbnail cache files
._*
Thumbs.db

# Files that might appear on external disks
.Spotlight-V100
.Trashes

# Files that might appear in the root of a volume
.DocumentRevisions-V100
.fseventsd
.TemporaryItems
.VolumeIcon.icns
.com.apple.timemachine.donotpresent

# Compiled Python files
*.pyc

# Compiled C++ files
*.out

# Application specific files
venv
node_modules
.vscode
.sass-cache
```

Or simply download [macOS specific .gitignore](https://github.com/github/gitignore/blob/master/Global/macOS.gitignore) maintained by GitHub itself and put contents of it to`~/.gitignore`.

> **Note**: You can also download it using curl
>
> ```text
> curl https://raw.githubusercontent.com/github/gitignore/master/Global/macOS.gitignore -o ~/.gitignore
> ```

If your gitignore file isn't working, you probably need to set up your global `core.excludesfile` configuration file to point to this global ignore file.

```text
git config --global core.excludesfile '~/.gitignore'
```

