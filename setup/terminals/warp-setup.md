---
description: The modern, AI-assisted terminal.
---

# Warp Setup



<figure><img src="../../.gitbook/assets/image (2) (1).png" alt="" width="563"><figcaption></figcaption></figure>

## Shell

### **Zsh**

Since macOS Catalina and higher, Zsh has been adopted replacing Bash. So no need to manually install zsh anymore. If you're not sure you can run `echo $SHELL` on your terminal and you should get `/bin/zsh` as a response.

### **Zsh Framework**

**Oh My Zsh** is an open-source, community-driven framework for managing your zsh configuration: [http://ohmyz.sh/](http://ohmyz.sh/)

#### Installation:

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

<figure><img src="../../.gitbook/assets/image (2).png" alt="" width="563"><figcaption></figcaption></figure>

## Prompt

[Pure prompt ](https://github.com/sindresorhus/pure)is a minimal, fast, and smart replacement for your terminal prompt in Zsh.&#x20;

**Install PURE via Homebrew:**

```zsh
brew install pure
```

**Add to your ZSH config**

* Open .zshrc by:

```
open -e ~/.zshrc
```

And add this to the end of your `~/.zshrc`:

```
# .zshrc
autoload -U promptinit; promptinit
prompt pure
```

{% hint style="info" %}
### **FAQ**

**What is a .zshrc file?** Basically, it’s a Z shell resource file that contains your configuration.

#### How do I edit/access the .zshrc file?

Your `.zshrc` file is in your home directory. To open it with your default text editor:

```
open ~/.zshrc
```

**Big Sur Issue: After installing Brew, I get a "command not found"**

Simply open your .zshrc file and add this:

`export PATH=/opt/homebrew/bin:$PATH`
{% endhint %}

## Zsh Plugins

### Zsh autosuggestions

[zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) is a [Fish](http://fishshell.com/)-like fast/unobtrusive auto-suggestions for zsh. It suggests commands as you type based on command history.

#### **Installation**:

```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

Search for the `plugins` line inside `~/.zshrc` and add the plugin to the list of plugins for Oh My Zsh to load

```
plugins=(git zsh-autosuggestions)
```

###

### Zsh Syntax Highlighting

[zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting) is a Fish shell-like syntax highlighting for Zsh.

#### Installation:

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

Then again, search for the `plugins` line inside `~/.zshrc` and add the plugin to the list of plugins for Oh My Zsh to load

```
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```

\
You need to `source` your config

```
source ~/.zshrc
```
