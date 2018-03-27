## Zsh

We'll install `zsh`for all the features offered by `oh-my-zsh`.

Install zsh and zsh-completions using Homebrew:

```
$ brew install zsh zsh-completions
```

Now let's use a framework built on top of this shell called `Oh My Zsh!`

#### Install Oh My Zsh!

Install [Oh My Zsh](http://ohmyz.sh/) on top of zsh to get additional functionality and super-charge your termnial!

```
$ curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh
```

If you're still in the default shell \(probably bash\), change default shell to zsh manually:

```
$ chsh -s /usr/local/bin/zsh
```

Restart your terminal, and confirm what shell you are actively using by typing in:

```
$ echo $SHELL
```

If it's not working, try restarting again.

#### Plugins

You can further extend zsh's power and functionalities by adding plugins to Oh My Zsh. There are useful plugins like completion plugins** **that will let `zsh` know which arguments the package has so it can autocomplete. You can manually select from [this plugins list](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins) and edit `~/.zshrc` then adding this line:

```
plugins=(
  git osx extract python ruby rails node npm
)
```

There are also plugins that goes beyond autocompleting - [check this list](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins-Overview) out. One of my picks are **extract **- for extracting zips in the terminal. This really depends on what you use/need so feel free to customize.

#### Homebrew Stuff To Do

One thing we need to do is tell the system to use programs installed by Homebrew \(in `/usr/local/bin`\) rather than the OS default if it exists. We do this by adding`/usr/local/bin`to your`$PATH`environment variable. Initially we we're using bash, but since we've switch to zsh, so we'll be editing the `.zshrc` instead of the `.bash_profile`

Now that we've already installed Oh My Zhs!

```
echo export PATH="/usr/local/bin:$PATH" >> ~/.zshrc
```

Alternatively, we can also insert`/usr/local/bin` to the first line of `/private/etc/paths` and reboot the Mac to change global paths loading order. Admin password may be required if you modify the file.

#### iTerm Color Schemes

Go to Preferences &gt; Profiles and Create your own color scheme! My personal favourite is the [Cobalt2 iTerm theme](https://github.com/wesbos/Cobalt2-iterm/blob/master/cobalt2.itermcolors), so download it. Got to Preferences &gt; Profiles &gt; Colors and import the `cobalt2.itermcolors` via Load Presets dropdown

#### Oh My Zsh Themes

While there are [alot of themes](https://github.com/robbyrussell/oh-my-zsh/wiki/themes) you can use with Oh My Zsh, my favourite is the [Cobalt2 theme](https://github.com/wesbos/Cobalt2-iterm). You can click on the theme link and follow the instructions there or follow thru here:

1. Open & edit your .zshrc file with `$ open .zshrc` then add & edit the following line `$ ZSH_THEME="cobalt2"`
2. Copy & paste the [cobalt2.zsh-theme](https://raw.githubusercontent.com/wesbos/Cobalt2-iterm/master/cobalt2.zsh-theme) file to `~/.oh-my-zsh/themes/`  directory

But wait, what are powerline fonts? These fonts are responsible for the icons you have on your terminal. There's actually [a directory of Powerline fonts](https://github.com/powerline/fonts) to choose from.

1. Install powerline `pip install --user powerline-status`
2. Clone the powerline fonts and run `install.sh` to install all powerline fonts

```
git clone https://github.com/powerline/fonts
```

```
cd fonts
./install.sh
```

Now head back to iTerm and go to Preferences &gt; Profiles &gt; Text and change the font style to 12pt Inconsolate for Powerline. You can play around with the size, change the powerline font - up to you guys :\)

Then refresh zsh by typing:

`source ~/.zshrc`

Or by restarting your terminal :\)

#### Shortcuts

`ctrl + a` to move at the beginning of the line

`ctrl + e` to move at the end of the line

`ctrl + u` to clear the current line

`ctrl + k` to clear all the characters that precedes the cursor position

`ctrl + l` to clear the screen

#### Frequently Asked Questions

**There's these weird \[?\] symbols on my terminal.** Probably missing the [powerline fonts](https://github.com/powerline/fonts)

**Where are my zsh settings stored? **`.zshrc`file located in your home directory. It’s a hidden file, so you might not see it in your home directory, but you can view it by running `open ~/.zshrc`from the terminal. Swap out `open`with your favorite editor command, such as `nano`, `subl`or `vim`. \(these are text editors, `nano` for [GNU Nano](https://www.nano-editor.org/), `subl` for [Sublime Text](https://www.sublimetext.com/), and `vim` for [Vim](http://www.vim.org/)\)

**It's not working! **Did you carefully follow the instructions? Don't copy the $ symbol on the commands. Also try restarting your terminal for it to take effect.

**I have no idea how to use the terminal / So hard to follow the instructions! **I suggest taking [this great course](https://commandlinepoweruser.com) by Wesbos.

