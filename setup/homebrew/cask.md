# Cask

[Homebrew Cask](https://caskroom.github.io/) is centered around installing GUI applications through the CLI. With Homebrew Cask, you can install the latest versions of applications by typing in a single command. Examples of these files is Google Chrome, Dropbox, VLC and Slack.

## Installation

As of December 2015, Cask comes installed with Homebrew, if you have not installed Homebrew see the

## Usage

To see if an app is available on Cask you can search on the [official Cask website](https://caskroom.github.io/search). You can also search using the following command:

```text
$ brew cask search <package>
```

To update brew and upgrade all install apps

```text
$ brew update && brew upgrade `brew outdated`
```

## App Suggestions

Here are some useful apps that are available on Cask.

```text
$ brew cask install \
    alfred \
    appcleaner \
    caffeine \
    cheatsheet \
    docker \
    dropbox \
    google-chrome \
    google-drive \
    google-hangouts \
    flux \
    1password \
    sublime-text \
    transmission \
    vlc
```

You can see more app suggestions on the last chapter \(and you can use brew cask to install them\).

