# Packages

### Trash

Not really a big fan of `rm` so heres a better alternative: [https://github.com/sindresorhus/trash](https://github.com/sindresorhus/trash)

#### Installation

You will need **Node** in order to install this package, to install Node:

```text
brew install node
```

And to install trash:

```text
npm install trash
```

{% hint style="info" %}
If you are already familiar with the folllowing below, here's a setup script that install everything below.
{% endhint %}

### Z

Z is actually not part of Zsh, but its a really cool way to jump to frecent folders. It makes navigating through the file system a breeze.

To install:

```text
brew install z
```

Also, don't forget to add this to your .zshrc file

```text
# include Z
. /usr/local/etc/profile.d/z.sh
```

### Youtube-dl

`Youtube-dl` is a command-line program used to download YouTube videos or videos from any platform in high resolution. There are also tons of other functionalities you can experiment with and you can check them out at their GitHub repository below.

```text
brew install youtube-dl
```

* Install ffmpeg: `brew install ffmpeg`
* Download highest-res: `youtube-dl -f bestvideo+bestaudio 'link'`
* Help:`youtube-dl —- help`

### Speedtest

`Speedtest-cli` is a command-line interface for testing internet bandwidth. It allows you to test against specific servers and even provides you with a URL so you can brag about your internet speed to your friends.

```text
brew install speedtest-cli
```

* Run: `speedtest-cli`

### Mac App Store CLI 

`mas` is a Mac App Store command-line interface that lets you install Mac apps from the App Store directly from the command line.

You can search for apps, install all existing updates, print the version number of an app in the store, and more. There’s even a fun option called lucky that will install the very first search result. Try it if you dare.

```text
brew install mas
```

* List all apps: `mas list`
* Search for apps: `mas search Xcode`
* Install apps: `mas install 497799835` \(the version number of the app\)
* Pending update apps: `mas outdated`
* Update apps: `mas upgrade`

### wifi-password

`wifi-password` does exactly what its name suggests, which is displaying the Wi-Fi password of the network you’re currently connected to. After inputting your Keychain authentication, the password shows up in bright green.

```text
brew install wifi-password
```

* Run: `wifi-password`

### Midnight-commander

`Midnight-commander` is a tool that amalgamates the functionality of the finder and command line, creating an interactive file manager in the terminal. Inside `Midnight-commander`, you can navigate your directory structure using clicks or the keyboard arrow.

```text
brew install midnight-commander
```

* Run: `mc`

[Midnight CommanderCurrent version is: 4.8.24; what's new. Coming soon: 4.8.25; what's new. Our release guidelines. GNU Midnight Commander…www.midnight-commander.org](https://www.midnight-commander.org/)

### htop

`htop` is an interactive system monitor, process viewer, and process manager for Unix, and it is said to be a successor to the Unix program `top`. It shows the updated list of processes running on your Mac and is ordered by the amount of CPU usage.

```text
brew install htop
```

* Run: `sudo htop`

### tree

`tree` is a tool that lists out the content of directories in a folder in a tree-like format. This useful trick is a life-saver for those who want a quick visual representation of a project’s file structure.

```text
brew install tree
```

* Run: `tree`

[The Tree Command for Linux HomepageDescription: Tree is a recursive directory listing command that produces a depth indented listing of files, which is…mama.indstate.edu](http://mama.indstate.edu/users/ice/tree/)

### archey

`archey` displays your system information inside the terminal along with a text-based retro-style Apple icon.

```text
brew install archey
```

* Run: `archey`
* Color: `archey -c`
* Black and white: `archey -b`

[Archey-osxEAn archey script for osXaobihann.github.io](https://obihann.github.io/archey-osx/)

### trash

`trash` is a simple program that moves files or folders to the trash.

```text
brew install trash
```

* Run: `trash [-vlesyF] <file> [<file> …]`
* Help: `trash —- help`

[trashThis page uses some Javascript; please turn it on in your browser. This is a small command-line program for OS X that…hasseg.org](https://hasseg.org/trash/)

## You-Get <a id="5c4c"></a>

[You-Get](https://you-get.org/) is similar to wget and youtube-dl combined, but with more flexible support for many more platforms and web formats. I use this often to grab videos from Twitter, Facebook, and even Instagram.

