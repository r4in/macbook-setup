---
description: The missing package manager for macOS
---

# Homebrew

![Updating GUI apps and packages has never been this easy](<../../.gitbook/assets/image (1) (1).png>)

> A package manager or package management system is a collection of software tools that automates the process of installing, upgrading, configuring, and removing computer programs for a computer's operating system in a consistent manner.

This is where we’ll be installing software packages like Git, Node.js, or Python. We can also install GUI apps such as Google Chrome, Slack, or VSCode.

{% hint style="warning" %}
**Why do you need this?**\
Homebrew works great for managing for automating the process of installing, upgrading, configuring software packages that you can't normally install using the App Store.&#x20;
{% endhint %}

## Installation

An important dependency before Homebrew can run is the **Command Line Tools for Xcode**, so make sure you’ve completed the previous step. These tools include compilers that allow you to build software from source. If you’re missing this, it’s available through **App Store > Updates**.

To install Homebrew, paste the following command into your Terminal, press **Enter**, and follow the on-screen instructions::

{% code overflow="wrap" %}
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
{% endcode %}

You might need to add Homebrew to your `PATH.` You can do so by entering these two commands:

{% code overflow="wrap" %}
```
(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/francisalturas/.zprofile
```
{% endcode %}

```
eval "$(/opt/homebrew/bin/brew shellenv)"
```

To start using Homebrew, you’ll need to open a new Terminal session. Do this by opening a new Terminal tab with Cmd+T (be sure to close the old one). Then, run the following command to ensure everything is working correctly:

```
brew doctor
```

After that, let's choose a terminal in the next section!

{% tabs %}
{% tab title="Usage" %}
To install a package (or **Formula** in Homebrew vocabulary) simply type:

```
brew install <formula_name_here>
```

#### Example

Install the [**Tree**](https://formulae.brew.sh/formula/tree) package which displays directories as trees in the terminal

```
brew install tree
```

After installing, give it a try!

```
tree /Applications
```

To update Homebrew's directory of formulae, run:

```
brew update
```

**Note**: I've seen that command fail sometimes because of a bug. If that ever happens, run the following (when you have Git installed):

```
cd /usr/local/Homebrew/
git fetch origin
git reset --hard origin/master
```

To see if any of your packages need to be updated:

```
brew outdated
```

To update a package:

```
brew upgrade <formula>
```

Homebrew keeps older versions of packages installed, in case you want to roll back. That rarely is necessary, so you can do some cleanup to get rid of those old versions:

```
brew cleanup
```

To see what you have installed (with their version numbers):

```
brew list --versions
```
{% endtab %}
{% endtabs %}

