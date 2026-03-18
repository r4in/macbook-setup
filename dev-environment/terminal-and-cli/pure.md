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

{% hint style="info" %}
### **FAQ**

**What is a .zshrc file?** Basically, it’s a Z shell resource file that contains your configuration.

#### How do I edit/access the .zshrc file?

Your `.zshrc` file is in your home directory. To open it with your default text editor:

```
open ~/.zshrc
```
{% endhint %}
