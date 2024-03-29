# Cask

[Homebrew Cask](https://caskroom.github.io/) is centered around installing GUI applications through the CLI. With this, you can install the latest versions of applications by typing in a single command. (like Google Chrome, Dropbox, VS Code and Slack)

### Usage

To see if an app is available on Cask you can search on the [official Cask website](https://caskroom.github.io/search). You can also search using the following command:

```
brew search <app-name-here>
```

To update brew and upgrade all install apps

```
brew update && brew upgrade `brew outdated`
```

## **Cask Upgrade**

[**Brew Cask Upgrade**](https://github.com/buo/homebrew-cask-upgrade) is a command-line tool for upgrading every outdated app installed by [Homebrew Cask](https://caskroom.github.io/).

To install, simple type

```
brew tap buo/cask-upgrade
```

To update all apps in one line:

```
brew cu -fa
```

