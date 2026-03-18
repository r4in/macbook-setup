---
description: The missing package manager for macOS
---

# Homebrew

<figure><img src="../../.gitbook/assets/image (45).png" alt="" width="375"><figcaption></figcaption></figure>

> A package manager is a tool that installs, updates, and manages software for you automatically.

[Homebrew](chatgpt://generic-entity?number=0) is the most popular **package** manager for macOS — think of it a command-line App Store for developers and power users. This is where we’ll be installing **packages** for **CLI tools** like Git, Node, or Python (aka "formula"). We can also install packages for **apps** like Figma, ChatGPT or Cursor. (Aka "cask")

{% hint style="warning" %}
**Why do you need this?**\
While you can use it to to install/manage software easily, Homebrew isn’t about installing apps — it’s about controlling your environment.
{% endhint %}

## Installation

To install Homebrew, paste the following command into your Terminal, press **Enter**, and follow the on-screen instructions:

```zsh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

You will also need to add Homebrew to your **PATH**. Follow the instructions on screen:

```zsh
echo >> ~/.zprofile
```

{% code overflow="wrap" %}
```zsh
echo 'eval "$(/opt/homebrew/bin/brew shellenv zsh)"' >> ~/.zprofile
```
{% endcode %}

```zsh
eval "$(/opt/homebrew/bin/brew shellenv zsh)"
```

{% hint style="info" %}
**What is PATH?**

PATH is a system variable that tells your Mac:

> “Where should I look for commands when you type something in Terminal?”


{% endhint %}

To start using Homebrew, you’ll need to open a new Terminal session. Do this by opening a new Terminal tab with `cmd + t` (be sure to close the old one). Then run the following command to ensure everything is working correctly:

```zsh
brew doctor
```

<figure><img src="../../.gitbook/assets/image (46).png" alt="" width="375"><figcaption></figcaption></figure>

After that, let's customize your terminal in the next section!
