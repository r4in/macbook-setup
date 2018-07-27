# Homebrew

[Homebrew](https://brew.sh/) a.k.a. **The missing package manager for macOS**

Why do you need this?

> A package manager or package management system is a collection of software tools that automates the process of installing, upgrading, configuring, and removing computer programs for a computer's operating system in a consistent manner.

This is where we'll be installing software packages such as Git, Node.js or Python. We can also install GUI apps such as Google Chrome, Slack or Skype.

## Installation

An important dependency before Homebrew can run is the **Command Line Tools** for **Xcode**. So make sure you completed the previous step. These include compilers that will allow you to build things from source, if you are missing this it's available through the App Store &gt; Updates.

To install Homebrew paste the following command in your **Terminal** \(without the dollar sign\), hit **Enter**, and follow the steps on the screen:

```text
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

To be able to use `brew` you need to start a new terminal session. Do this by opening a new terminal tab with **Cmd+T** \(you should also close the old one\), then run the following command to make sure everything is working:

```text
$ brew doctor
```



