## Zsh

We'll install`zsh`for all the features offered by`oh-my-zsh`. The installation and usage is really intuitive. We will also create the file`env.sh`, it is a config file we maintain so as to not pollute the`~/.zshrc`too much.`env.sh`holds aliases, exports, path changes etc. and you can find it at the bottom of this page.

Install zsh and zsh-completions using Homebrew:

```
$ brew install zsh zsh-completions
```

Now let's use a framework built on top of this shell called `Oh My Zsh!`

#### Install Oh My Zsh

Install Oh My Zsh on top of zsh to get additional functionality:

```
$ curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh
```

If you're still in the default shell \(probably bash\), change default shell to zsh manually:

```
$ chsh -s /usr/local/bin/zsh
```

You can confirm what shell you are actively using by typing in:

```
$ echo $SHELL
```

If it's not working, try restarting your terminal.

#### Themes & Customizations

While there are [alot of themes](https://github.com/robbyrussell/oh-my-zsh/wiki/themes) you can use with Oh My Zsh, my favourite is the [Cobalt2 theme](https://github.com/wesbos/Cobalt2-iterm).

#### Plugins

You can add plugins to Oh My Zsh by selecting from [this list](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins) and by editing`~/.zshrc `and adding:

```
plugins=(
  git osx
)
```

[Check this out for more info](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins)

#### Frequently Asked Questions

**I'm missing a few fonts!** Probably missing the [powerline fonts](https://github.com/powerline/fonts)

**Where are my zsh settings stored? **`.zshrc`file located in your home directory. It’s a hidden file, so you might not see it in your home directory, but you can view it by running `open ~/.zshrc`from the terminal. Swap out `open`with your favorite editor command, such as `nano`, `subl`or `vim`.

**It's not working! **Try restarting your terminal for it to take effect.

**I have no idea how to use the terminal / So hard to follow the instructions! **I suggest taking [this great course](https://commandlinepoweruser.com) by Wesbos.

