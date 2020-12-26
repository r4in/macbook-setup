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

#### Installation

```text
brew install z
```

Also, don't forget to add this to your .zshrc file

```text
# include Z
. /usr/local/etc/profile.d/z.sh
```

#### Usage

```text
z <folder or app name>
```

### Youtube-dl

`Youtube-dl` is a command-line program used to download YouTube videos or videos from any platform in high resolution. There are also tons of other functionalities you can experiment with and you can check them out at their GitHub repository below.

```text
brew install youtube-dl
```

#### Installation

```text
brew install ffmpeg
```

#### Usage

* Download highest-res: `youtube-dl -f bestvideo+bestaudio 'link'`
* Help:`youtube-dl —- help`



### Speedtest

`Speedtest-cli` is a command-line interface for testing internet bandwidth. It allows you to test against specific servers and even provides you with a URL so you can brag about your internet speed to your friends.

#### Installation

```text
brew install speedtest-cli
```

#### Usage

```text
speedtest-cli
```



### Mac App Store CLI 

`mas` is a Mac App Store command-line interface that lets you install Mac apps from the App Store directly from the command line.

You can search for apps, install all existing updates, print the version number of an app in the store, and more. There’s even a fun option called lucky that will install the very first search result. Try it if you dare.

#### Installation

```text
brew install mas
```

#### Usage

* List all apps: `mas list`
* Search for apps: `mas search Xcode`
* Install apps: `mas install 497799835` \(the version number of the app\)
* Pending update apps: `mas outdated`
* Update apps: `mas upgrade`



### wifi-password

`wifi-password` does exactly what its name suggests, which is displaying the Wi-Fi password of the network you’re currently connected to. After inputting your Keychain authentication, the password shows up in bright green.

#### Installation

```text
brew install wifi-password
```

#### Usage

```text
wifi-password
```



### tree

`tree` is a tool that lists out the content of directories in a folder in a tree-like format. This useful trick is a life-saver for those who want a quick visual representation of a project’s file structure.

#### Installation

```text
brew install tree
```

#### Usage

```text
tree
```



### archey

`archey` displays your system information inside the terminal along with a text-based retro-style Apple icon.

#### Installation

```text
brew install archey
```

#### Usage

* Run: `archey`
* Color: `archey -c`
* Black and white: `archey -b`

{% hint style="warning" %}
I forgot which medium article I got some of these from. Credits to their respective owners. Feel free to DM so I can attribute you. Thanks!
{% endhint %}

