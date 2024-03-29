# Hyper Setup

Hyper is an Electron-based terminal built on HTML/CSS/JS. I like how less configurations I need to do to start doing my work. Credits to [@cesarmcferreira](https://twitter.com/cesarmcferreira) for this neat setup.

To install, simply run the following in your terminal:

```
brew install hyper
```

After installing, open **Hyper** and use it for the rest of the setup.

### Theme

**hyper snazzy** an elegant Hyper theme with bright colors [https://github.com/sindresorhus/hyper-snazzy](https://github.com/sindresorhus/hyper-snazzy)

_You'll need to install the PURE prompt installed first before proceeding_

```
hyper install hyper-snazzy
```

## Shell

### **Zsh**

Since macOS Catalina and higher, Zsh has been adopted replacing Bash. So no need to manually install zsh anymore. If you're not sure you can run `echo "$SHELL"` on your terminal and you should get `/bin/zsh` as a response.

### **Zsh Framework**

**Oh-my-zsh** is an open-source, community-driven framework for managing your zsh configuration [http://ohmyz.sh/](http://ohmyz.sh/)

#### Installation:

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## Prompt

**Pure** is a pretty, minimal, and fast ZSH prompt [https://github.com/sindresorhus/pure](https://github.com/sindresorhus/pure)

But you'll need node installed first:

```
brew install node
```

Then, to install:

```
npm install --global pure-prompt
```

And add this to the end of your `~/.zshrc`

```
# .zshrc
autoload -U promptinit; promptinit
prompt pure
```

{% hint style="info" %}
### **FAQ**

**What is a .zshrc file?** Basically, it's a Z-shell resource that contains all your configurations.

#### How do I edit / access the .zshrc file?

Your .zshrc file is usually located at the root. To open, use your default text editor:

```
open ~/.zshrc
```

**Big Sur Issue: After installing Brew, I get a "command not found"**

Simply open your .zshrc file and add this:

`export PATH=/opt/homebrew/bin:$PATH`
{% endhint %}

## Zsh Plugins

### Zsh autosuggestions

[zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) is a [Fish](http://fishshell.com/)-like fast/unobtrusive autosuggestions for zsh. It suggests commands as you type based on command history.

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

[zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting) is a Fish shell like syntax highlighting for Zsh.

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

