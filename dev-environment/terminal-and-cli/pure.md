# Pure

## Pure

Pure is a minimal, fast, and modern command-line prompt for Zsh—basically the UI you see in your terminal before you type commands.

To install:

```
brew install pure
```

Then add this to the end of your `~/.zshrc`  file:

```
fpath+=("$(brew --prefix)/share/zsh/site-functions")
autoload -U promptinit; promptinit
prompt pure
```
