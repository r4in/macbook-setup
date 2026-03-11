# Hyper Setup

Hyper is an Electron-based terminal built on HTML/CSS/JS. I like how few configuration changes I need to start working. Credits to [@cesarmcferreira](https://twitter.com/cesarmcferreira) for this neat setup.

To install, simply run the following in your terminal:

```
brew install hyper
```

After installing, open **Hyper** and use it for the rest of the setup.

### Theme

**hyper snazzy** is an elegant Hyper theme with bright colors: [https://github.com/sindresorhus/hyper-snazzy](https://github.com/sindresorhus/hyper-snazzy)

_You’ll need to install the Pure prompt first before proceeding._

```
hyper install hyper-snazzy
```

## Shell

### **Zsh**

Since macOS Catalina, Zsh has been adopted as the default shell, replacing Bash. So there’s no need to manually install Zsh anymore. If you’re not sure, run `echo "$SHELL"` in your terminal. You should get `/bin/zsh` as a response.

### **Zsh Framework**

**Oh My Zsh** is an open-source, community-driven framework for managing your Zsh configuration: [http://ohmyz.sh/](http://ohmyz.sh/)

#### Installation:

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## Prompt

**Pure** is a pretty, minimal, and fast Zsh prompt: [https://github.com/sindresorhus/pure](https://github.com/sindresorhus/pure)

But you’ll need Node installed first:

```
brew install node
```

Then, to install:

```
npm install --global pure-prompt
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

#### How do I edit / access the .zshrc file?

Your `.zshrc` file is in your home directory. To open it, use your default text editor:

```
open ~/.zshrc
```

**Big Sur Issue: After installing Brew, I get a "command not found"**

Simply open your .zshrc file and add this:

`export PATH=/opt/homebrew/bin:$PATH`
{% endhint %}

## Zsh Plugins

### Zsh autosuggestions

[zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) is a [Fish](http://fishshell.com/)-like, fast, unobtrusive auto-suggestion plugin for Zsh. It suggests commands as you type, based on your command history.

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

[zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting) is a Fish shell-like syntax highlighting plugin for Zsh.

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
