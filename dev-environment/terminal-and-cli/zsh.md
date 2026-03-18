# Zsh

## **Zsh**

Since macOS Catalina and higher, Zsh has been adopted replacing Bash. So no need to manually install zsh anymore. If you're not sure you can run `echo $SHELL` on your terminal and you should get `/bin/zsh` as a response.

***

## **Oh My Zsh**

**Oh My Zsh** is an open-source, community-driven framework for managing your zsh configuration: [http://ohmyz.sh/](http://ohmyz.sh/)

**Installation:**

```zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

<figure><img src="../../.gitbook/assets/image (50).png" alt="" width="563"><figcaption></figcaption></figure>

***

## Plugins

#### Zsh autosuggestions

[zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) is a [Fish](http://fishshell.com/)-like fast/unobtrusive auto-suggestions for zsh. It suggests commands as you type based on command history.

**Installation**:

```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

Search for the `plugins` line inside `~/.zshrc` and add the plugin to the list of plugins for Oh My Zsh to load

```
plugins=(git zsh-autosuggestions)
```

### Zsh Syntax Highlighting

[zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting) is a Fish shell-like syntax highlighting for Zsh.

**Installation:**

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
