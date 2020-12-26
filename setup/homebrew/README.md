---
description: The missing package manager for macOS
---

# Homebrew

![Updating GUI apps and packages has never been this easy](../../.gitbook/assets/image%20%281%29.png)

> A package manager or package management system is a collection of software tools that automates the process of installing, upgrading, configuring, and removing computer programs for a computer's operating system in a consistent manner.

This is where we'll be installing software packages such as Git, Node.js or Python. We can also install GUI apps such as Google Chrome, Slack or Skype.

{% hint style="warning" %}
**Why do you need this?**  
Homebrew works great for managing for automating the process of installing, upgrading, configuring software packages that you can't normally install using the App Store. 
{% endhint %}

## Installation

An important dependency before Homebrew can run is the **Command Line Tools** for **Xcode**. So make sure you completed the previous step. These include compilers that will allow you to build things from source, if you are missing this it's available through the **App Store &gt; Updates.**

To install Homebrew paste the following command in your **Terminal** and hit enter, and follow the steps on the screen:

```text
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

To be able to use `brew` you need to start a new terminal session. Do this by opening a new terminal tab with **Cmd+T** \(you should also close the old one\), then run the following command to make sure everything is working:

```text
brew doctor
```

After that, let's choose a terminal in the next section!

{% tabs %}
{% tab title="Usage" %}
To install a package \(or **Formula** in Homebrew vocabulary\) simply type:

```text
brew install <formula_name_here>
```

#### Example

Install the [**Tree**](https://formulae.brew.sh/formula/tree) package which displays directories as trees in the terminal

```text
brew install tree
```

After installing, give it a try!

```text
tree /Applications
```

To update Homebrew's directory of formulae, run:

```text
brew update
```

**Note**: I've seen that command fail sometimes because of a bug. If that ever happens, run the following \(when you have Git installed\):

```text
cd /usr/local/Homebrew/
git fetch origin
git reset --hard origin/master
```

To see if any of your packages need to be updated:

```text
brew outdated
```

To update a package:

```text
brew upgrade <formula>
```

Homebrew keeps older versions of packages installed, in case you want to roll back. That rarely is necessary, so you can do some cleanup to get rid of those old versions:

```text
brew cleanup
```

To see what you have installed \(with their version numbers\):

```text
brew list --versions
```
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}

