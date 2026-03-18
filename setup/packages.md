# Terminal Packages

Below are some recommended packages that are helpful to have in your selected terminal.

{% hint style="info" %}
If you are already familiar with the packages listed, here's a shell script that installs everything below. [https://github.com/r4in/shellscripts/blob/master/packages.sh](https://github.com/r4in/shellscripts/blob/master/packages.sh)
{% endhint %}

## Trash

Not really a big fan of `rm`, so here’s a better alternative: [https://github.com/sindresorhus/trash](https://github.com/sindresorhus/trash)

#### Installation

You will need **Node** to install this package. To install Node:

```
brew install node
```

And to install trash:

```
npm install trash
```

## Z

Z is not part of Zsh, but it’s a really cool way to jump to “frecent” folders. It makes navigating the file system a breeze.

#### Installation

```
brew install z
```

Also, don’t forget to add this to your `.zshrc` file:

```
# include Z
. /usr/local/etc/profile.d/z.sh
```

#### Usage

```
z <folder or app name>
```

## youtube-dl

`youtube-dl` is a command-line program used to download YouTube videos (and videos from other platforms) in high resolution. There are tons of other features you can experiment with. Check the GitHub repo below.

```
brew install youtube-dl
```

#### Installation

```
brew install ffmpeg
```

#### Usage

* Download highest-res: `youtube-dl -f bestvideo+bestaudio 'link'`
* Help: `youtube-dl --help`

## Speedtest

`Speedtest-cli` is a command-line interface for testing internet bandwidth. It allows you to test against specific servers and even provides you with a URL so you can brag about your internet speed to your friends.

#### Installation

```
brew install speedtest-cli
```

#### Usage

```
speedtest-cli
```

## Mac App Store CLI

`mas` is a Mac App Store command-line interface that lets you install Mac apps from the App Store directly from the command line.

You can search for apps, install all existing updates, print the version number of an app in the store, and more. There’s even a fun option called lucky that will install the very first search result. Try it if you dare.

#### Installation

```
brew install mas
```

#### Usage

* List all apps: `mas list`
* Search for apps: `mas search Xcode`
* Install apps: `mas install 497799835` (the version number of the app)
* Pending update apps: `mas outdated`
* Update apps: `mas upgrade`

## tree

`tree` is a tool that lists out the content of directories in a folder in a tree-like format. This useful trick is a life-saver for those who want a quick visual representation of a project’s file structure.

#### Installation

```
brew install tree
```

#### Usage

```
tree
```

## archey

`archey` displays your system information inside the terminal along with a text-based retro-style Apple icon.

#### Installation

```
brew install archey
```

#### Usage

* Run: `archey`
* Color: `archey -c`
* Black and white: `archey -b`
