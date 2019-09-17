# Sublime Text

[Sublime Text](http://www.sublimetext.com/) is a sophisticated text editor for code, markup and prose. You'll love the slick user interface, extraordinary features and amazing performance.

## Installation <a id="installation"></a>

[Download](http://www.sublimetext.com/) the **.dmg** file and drag-and-drop it to the **Applications** folder or simply

```text
brew install sublime-text
```

## Use CLI to open file <a id="use-cli-to-open-file"></a>

Let's create a shortcut so we can launch Sublime Text from the command-line

```text
ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
```

Now you can open a file with`subl myfile.py`or start a new project in the current directory with`subl .`

