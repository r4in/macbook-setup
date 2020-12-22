# Tech Stack

## Ruby

macOS comes with Ruby installed, but as we don't want to be messing with operating system core files we could use the tools `rbenv`and `ruby-build`to manage and install our Ruby versions for our development environment.

## Python

macOS, like Linux, ships with [Python](http://python.org/) already installed. But you don't want to mess with the system Python \(some system tools rely on it, etc.\), so we'll install our own version\(s\). There are two ways to install Python, \(1\) Homebrew and \(2\) Pyenv. If you plan to use multiple versions of Python \(e.g. 2, 3, and anaconda\) then you should use pyenv.

## npm & nodejs

npm makes it easy for JavaScript developers to share and reuse code, and makes it easy to update the code that you’re sharing, so you can build amazing things.

npm is distributed with [Node.js](https://nodejs.org/)- which means that when you download Node.js, you automatically get npm installed on your computer.

```text
brew cask install node
```

## Sass

while there are alot of apps out there that get you up and running with sass, either with an application \(codekit, prepros\), or the command line. Sass has a ruby dependecy on OSX, you can immediately type in:

```text
sudo gem install sass
```

but i usually use the gulp-sass npm package and rarely use the system-wide one.

## Google Cloud

Most of our web apps run on Google Cloud Platform which lets you build and host applications and websites, store data, and analyze data on Google's scalable infrastructure.

Visit this site and follow the instructions: [https://cloud.google.com/sdk/docs/quickstart-macos](https://cloud.google.com/sdk/docs/quickstart-macos)

