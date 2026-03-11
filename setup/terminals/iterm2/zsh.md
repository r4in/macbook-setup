# Zsh

{% hint style="info" %}
Announced in June and released in October 2019, [macOS Catalina](https://en.wikipedia.org/wiki/MacOS_Catalina) adopted Zsh as the default shell, replacing [Bash](https://en.wikipedia.org/wiki/Bash_\(Unix_shell\)). Although the copy of Zsh available on macOS by default is the one that shipped with the system, it will eventually get out of date. So the first thing to do is install the latest version with Homebrew.
{% endhint %}

So that means no need to manually install Zsh anymore! 🥳

Install zsh and zsh-completions using Homebrew:

```
brew install zsh zsh-completions
```

After installation, you’ll come across this message:

![](<../../../.gitbook/assets/Screen Shot 2019-12-30 at 9.29.06 PM.png>)

Add `fpath=(path/to/zsh-completions/src $fpath)` to your **.zshrc** file. However, it will still get overwritten when we install Oh My Zsh (I’ll explain later), so we’ll come back to this in the next step.

Now let's use a framework built on top of this shell called **Oh My Zsh!**

## Shell

### Oh My Zsh

Install [Oh My Zsh](http://ohmyz.sh/) on top of Zsh to get additional functionality and supercharge your terminal!

```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

#### Resolving the issue from the previous step

Let’s open the **.zshrc** file using Sublime Text:

```
subl ~/.zshrc
```

Then copy-paste this text and save the file:

```
fpath=(path/to/zsh-completions/src $fpath)
```

Then go back to Terminal and run this:

```
rm -f ~/.zcompdump; compinit
```

## Plugins

You can further extend Zsh’s power by adding plugins to Oh My Zsh. Completion plugins let `zsh` know which arguments a command supports, so it can autocomplete.

**What is a .zshrc file?** Basically, it’s a Zsh resource file that contains your configuration.

### How do I edit/access the .zshrc file?

Your `.zshrc` file is in your home directory. To open it, use your default text editor:

```
open ~/.zshrc
```

### **How to add plugins?**

To add a plugin, update the `plugins` list in your **.zshrc** file. Example:

```
plugins=(
  git osx extract python ruby rails node npm
)
```

You can also manually select things you want to add from [this plugins list](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins).

## Homebrew Stuff To Do

One thing we need to do is tell the system to use programs installed by Homebrew (in `/usr/local/bin`) rather than the OS default, if it exists. We do this by adding `/usr/local/bin` to your `$PATH` environment variable.

Now that we’ve installed Oh My Zsh, this command will append `PATH="/usr/local/bin:$PATH"` to your `.zshrc` file:

```
echo export PATH="/usr/local/bin:$PATH" >> ~/.zshrc
```

## iTerm Color Schemes

Open iTerm, go to **Preferences > Profiles** and create your own color scheme!

My personal favorite is the [Cobalt2 iTerm theme](https://github.com/wesbos/Cobalt2-iterm/blob/master/cobalt2.itermcolors). To use it:

1. Download [cobalt2.itermcolors](https://raw.githubusercontent.com/wesbos/Cobalt2-iterm/master/cobalt2.itermcolors)
2. Go to **Preferences > Profiles** and click on the "**+**" button to add a new profile.
3. Give it a name, and click on the **Colors** tab
4. Import **cobalt2.itermcolors** by clicking on the **Color Presets..** > **Import..**
5. After importing, select **Color Presets..** > **cobalt2**

![](<../../../.gitbook/assets/Screen Shot 2019-12-30 at 10.22.32 PM.png>)

## Oh My Zsh Themes

While there are [a lot of themes](https://github.com/robbyrussell/oh-my-zsh/wiki/themes) you can use with Oh My Zsh, my favorite is the [Cobalt2 theme](https://github.com/wesbos/Cobalt2-iterm). You can click on the theme link and follow the instructions there or follow through here:

1. Open & edit your .zshrc file with `$ open .zshrc` then search & modify the following line `$ ZSH_THEME="cobalt2"`
2. Copy & paste the [cobalt2.zsh-theme](https://raw.githubusercontent.com/wesbos/Cobalt2-iterm/master/cobalt2.zsh-theme) file to `~/.oh-my-zsh/themes/` directory

## Powerline

What is [**Powerline**](https://github.com/powerline/powerline)? It’s a statusline plugin for Vim. It provides status lines and prompts. Along with it are [**Powerline Fonts**](https://github.com/powerline/fonts), which are responsible for the icons in your terminal. To enable Powerline fonts on the theme we’re using:

Powerline uses `pip` (a package manager for Python).

* Install **Powerline**

```
pip3 install --user powerline-status
```

* Clone the [Powerline fonts](https://github.com/powerline/fonts) and run `install.sh` to install all powerline fonts

```
git clone https://github.com/powerline/fonts
cd fonts
./install.sh
```

Now head back to iTerm and go to **Preferences** > **Profiles** > **Text** and change the font family to **Inconsolata for Powerline**, font weight to **Medium,** and set the font size to **12px**. Then you should be seeing icons in your command prompt like this:

![](<../../../.gitbook/assets/Screen Shot 2019-12-31 at 12.31.00 AM.png>)

{% hint style="info" %}
You can play around with the size and change the Powerline font — up to you 😄
{% endhint %}

Then refresh Zsh by typing `source ~/.zshrc` or by restarting your terminal.

## Shortcuts

`ctrl + a` to move at the beginning of the line

`ctrl + e` to move at the end of the line

`ctrl + u` to clear the current line

`ctrl + k` to clear all the characters that precedes the cursor position

`ctrl + l` to clear the screen

## Frequently Asked Questions

**There are weird \[?] symbols on my terminal.** You’re probably missing the [Powerline fonts](https://github.com/powerline/fonts).

**Where are my Zsh settings stored?** In the `.zshrc` file in your home directory. It’s hidden, so you might not see it in Finder. You can open it by running `open ~/.zshrc` from Terminal. Swap out `open` with your preferred editor command, such as `nano`, `subl`, or `vim`. (These are text editors: `nano` for [GNU Nano](https://www.nano-editor.org/), `subl` for [Sublime Text](https://www.sublimetext.com/), and `vim` for [Vim](http://www.vim.org/).)

**It’s not working!** Did you carefully follow the instructions? Also try restarting your terminal for it to take effect.

**I have no idea how to use the terminal / So hard to follow the instructions!** I suggest taking [this great course](https://commandlinepoweruser.com) by Wesbos.\
\
**When I open my terminal this message shows up:**`compdef: unknown command or service: rails`\
\
Just run this and it should be working fine:

```
rm -f ~/.zcompdump*; compinit
```
