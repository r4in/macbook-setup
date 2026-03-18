# Git Ignore

Create the file `~/.gitignore` as shown below, so you don’t track files that are almost always ignored in Git repositories.

```
touch ~/.gitignore
```

Open the `.gitignore` file using your favorite text editor and add the following:

```
# Folder view configuration files
.DS_Store
Desktop.ini
.LSOverride

# Icon must end with two \r
Icon

# Thumbnail cache files
._*
Thumbs.db

# Files that might appear on external disks
.Spotlight-V100
.Trashes

# Files that might appear in the root of a volume
.DocumentRevisions-V100
.fseventsd
.Spotlight-V100
.TemporaryItems
.Trashes
.VolumeIcon.icns
.com.apple.timemachine.donotpresent

# Directories potentially created on remote AFP share
.AppleDB
.AppleDesktop
Network Trash Folder
Temporary Items
.apdisk

# Compiled Python files
*.pyc

# Compiled C++ files
*.out

# Application-specific files
venv
node_modules
.vscode
.sass-cache
```

Or download the [macOS-specific .gitignore](https://github.com/github/gitignore/blob/master/Global/macOS.gitignore) maintained by GitHub, then copy its contents into `~/.gitignore`.

> **Note**: You can also download it using curl
>
> ```
> curl https://raw.githubusercontent.com/github/gitignore/master/Global/macOS.gitignore -o ~/.gitignore
> ```

If your `.gitignore` file isn’t working, you probably need to set up your global `core.excludesfile` config to point to this global ignore file.

```
git config --global core.excludesfile '~/.gitignore'
```
