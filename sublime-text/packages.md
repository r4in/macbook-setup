#### Install Package Control

The simplest method of installation is through the Sublime Text console. The console is accessed via`View > Show Console`menu or simple hit \`\`ctrl + \`\`\` and paste this in the console:

```
import urllib.request,os,hashlib; h = '6f4c264a24d933ce70df5dedcf1dcaee' + 'ebe013ee18cced0ef93d5f746d80ef60'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

This snippet changes each version and older versions will return an error.

To get the current versions code, go to [https://packagecontrol.io/installation](https://packagecontrol.io/installation)

#### Install Packages 

[Alignment](https://github.com/wbond/sublime_alignment/issues): Easy alignment of multiple selections and multi-line selections

[All Autocomplete](https://github.com/alienhard/SublimeAllAutocomplete): Extend Sublime Text 2 auto-completion to find matches in all open files of the current window

[AutoFileName](https://github.com/BoundInCode/AutoFileName): Plugin that auto-completes filenames

[Bootstrap 3 Snippets](https://github.com/JasonMortonNZ/bs3-sublime-plugin): Twitter Bootstrap 3 snippets plugin for Sublime Text 2 and 3

[BracketHighlighter](https://github.com/facelessuser/BracketHighlighter): Bracket and tag highlighter

[Dictionaries](https://github.com/SublimeText/Dictionaries): Hunspell UTF8 dictionaries

[DictionaryAutoComplete](https://github.com/Zinggi/DictionaryAutoComplete): Plugin that adds dictionary entries to the completions inside comments

[EncodingHelper](https://github.com/SublimeText/EncodingHelper): Guess encoding of files, show in status bar, convert to UTF-8 from a variety of encodings

[FileDiffs](https://github.com/colinta/SublimeFileDiffs): Shows diffs between the current file, or selection\(s\) in the current file, and clipboard, another file, or unsaved changes

[Git](https://github.com/kemayo/sublime-text-git): Plugin for some Git integration

[GitGutter](http://www.jisaacks.com/gitgutter): A Sublime Text 2 and 3 plugin to see git diff in gutter

[IndentXML](https://github.com/alek-sys/sublimetext_indentxml): Plugin for re-indenting XML and JSON files

[Jade](https://github.com/davidrios/jade-tmbundle): A comprehensive bundle for the Jade template language

[Jedi - Python autocompletion](https://github.com/srusskih/SublimeJEDI): Jedi is an autocompletion tool for Python

[Jekyll](https://github.com/23maverick23/sublime-jekyll): A plugin for Jekyll static sites

[LaTeXTools](https://github.com/SublimeText/LaTeXTools): A LaTeX Plugin for Sublime Text 2 and 3

[Python Auto-Complete](https://github.com/eliquious/Python-Auto-Complete): Sublime Text 2 plugin which adds additional auto-completion capability to Python scripts

[Python Imports Sorter](https://github.com/vi4m/sublime_python_imports): Sublime Text 2 plugin to organize your imports easily

[Python PEP8 Autoformat](https://bitbucket.org/StephaneBunel/pythonpep8autoformat): Python PEP8 auto-format is a plugin to interactively reformat Python source code according to PEP-8

[PythonTraceback](https://github.com/kedder/sublime-python-traceback): Easy navigation in your python tracebacks

[SideBarEnhancements](https://github.com/titoBouzout/SideBarEnhancements): Enhancements to sidebar. Files and folders.

[SublimeCodeIntel](http://sublimecodeintel.github.io/SublimeCodeIntel/): Full-featured code intelligence and smart auto-complete engine

[SublimeLinter](http://sublimelinter.readthedocs.org/): Interactive code linting framework for Sublime Text 3

[SublimeLinter-pep8](https://github.com/SublimeLinter/SublimeLinter-pep8): Linter plugin for python using PEP8

[TrailingSpaces](https://github.com/SublimeText/TrailingSpaces): Highlight trailing spaces and delete them in a flash

#### Install Themes

You can simple yo to package control and search for themes. I would recommend using the [Material theme](https://github.com/equinusocio/material-theme) or [Brogrammer Theme](https://github.com/kenwheeler/brogrammer-theme).



