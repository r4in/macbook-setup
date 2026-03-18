# Zsh

## **Zsh**

Zsh (Z Shell) is a command-line shell — the program that lets you interact with your computer by typing commands. Think of it as the engine behind your terminal.

Since macOS Catalina and higher, Zsh has been adopted replacing Bash. So there's no need to manually install `zsh` anymore. If you're not sure, you can run `echo $SHELL` on your terminal and you should get `/bin/zsh` as a response.

***

## **Oh My Zsh**

Oh My Zsh is a framework that helps you manage and customize Zsh (your terminal shell).

**Installation:**

```zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

<figure><img src="../../.gitbook/assets/image (50).png" alt="" width="563"><figcaption></figcaption></figure>

***

## Plugins

#### Zsh Autosuggestions

zsh-autosuggestions is a plugin for Zsh that suggests commands as you type, based on your history.

**Installation**:

```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

Search for the `plugins` line inside `~/.zshrc` and add the plugin to the list of plugins for Oh My Zsh to load

```
plugins=(git zsh-autosuggestions)
```

#### Zsh Syntax Highlighting

Zsh Syntax Highlighting is a plugin that colors your terminal commands as you type, so you can instantly see if something is valid or wrong.

**Installation:**

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

Then again, search for the `plugins` line inside `~/.zshrc` and add the plugin to the list of plugins for Oh My Zsh to load

```
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```

\
Then reload your zsh configuration file by running:

```
source ~/.zshrc
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
