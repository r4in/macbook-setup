# Cask

[Homebrew Cask](https://caskroom.github.io/) is an extension of [Homebrew](chatgpt://generic-entity?number=0) that lets you install macOS apps (GUI apps) from the terminal — not just command-line tools.

### Usage

Instead of:

* going to a website
* downloading a .dmg
* dragging to Applications

You just run:

```zsh
brew install --cask google-chrome
```

And it:

* downloads the app
* installs it in /Applications
* keeps it manageable via Brew

To see if an app is available on Cask, search the [official Cask website](https://caskroom.github.io/search). You can also search using the following command:

```
brew search <app-name-here>
```

To update Homebrew and upgrade all installed apps:

```
brew update && brew upgrade `brew outdated`
```

## **Cask Upgrade**

[**Brew Cask Upgrade**](https://github.com/buo/homebrew-cask-upgrade) is a command-line tool for upgrading every outdated app installed by [Homebrew Cask](https://caskroom.github.io/).

To install, simply type:

```
brew tap buo/cask-upgrade
```

To update all apps in one line:

```
brew cu -fa
```
