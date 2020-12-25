# Hyper Setup

Hyper is an Electron-based terminal built on HTML/CSS/JS. I like how less configurations I need to do to start doing my work. Credits to [@cesarmcferreira](https://twitter.com/cesarmcferreira) for this neat setup.

### Installation

To install, simply run the following in your terminal:

```text
brew install hyper
```

## Theme

**hyper snazzy** an elegant Hyper theme with bright colors [https://github.com/sindresorhus/hyper-snazzy](https://github.com/sindresorhus/hyper-snazzy)

```text
hyper install hyper-snazzy
```

## Shell

**Oh-my-zsh** is an open source, community-driven framework for managing your zsh configuration [http://ohmyz.sh/](http://ohmyz.sh/)

```text
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### Prompt

**Pure** is a pretty, minimal and fast ZSH prompt [https://github.com/sindresorhus/pure](https://github.com/sindresorhus/pure)

But you'll need node installed first:

```text
brew install node
```

Then, to install:

```text
npm install --global pure-prompt
```

And add this to the end of your ~/.zshrc

```text
# .zshrc
autoload -U promptinit; promptinit
prompt pure
```

##  <a id="d7f5"></a>

### Oh My Zsh

1. Clone this repository into `$ZSH_CUSTOM/plugins` \(by default `~/.oh-my-zsh/custom/plugins`\)

   ```text
   git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
   ```

2. Add the plugin to the list of plugins for Oh My Zsh to load \(inside `~/.zshrc`\):

   ```text
   plugins=(zsh-autosuggestions)
   ```

3. Start a new terminal session.

##  <a id="7681"></a>

## Zsh autosuggestions <a id="d7f5"></a>

[zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) is a [Fish](http://fishshell.com/)-like fast/unobtrusive autosuggestions for zsh. It suggests commands as you type based on command history.

### **Installation**: <a id="d79b"></a>

```text
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

## Zsh Syntax Highlighting <a id="7681"></a>

[zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting) is a Fish shell like syntax highlighting for Zsh.

### Installation: <a id="2bbf"></a>

```text
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

## ZSH plugins <a id="fa2e"></a>

From my `~/.zshrc`

> plugins=\(git osx **zsh-autosuggestions** **zsh-syntax-highlighting**\)

You need to `source` your config

```text
source ~/.zshrc
```

