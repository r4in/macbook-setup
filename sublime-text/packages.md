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

[BracketHighlighter](https://github.com/facelessuser/BracketHighlighter): Bracket and tag highlighter

[FileDiffs](https://github.com/colinta/SublimeFileDiffs): Shows diffs between the current file, or selection\(s\) in the current file, and clipboard, another file, or unsaved changes

[Git](https://github.com/kemayo/sublime-text-git): Plugin for some Git integration

[SideBarEnhancements](https://github.com/titoBouzout/SideBarEnhancements): Enhancements to sidebar. Files and folders.

[SublimeCodeIntel](http://sublimecodeintel.github.io/SublimeCodeIntel/): Full-featured code intelligence and smart auto-complete engine

[SublimeLinter](http://sublimelinter.readthedocs.org/): Interactive code linting framework for Sublime Text 3

[TrailingSpaces](https://github.com/SublimeText/TrailingSpaces): Highlight trailing spaces and delete them in a flash

#### Install Themes

You can simple go to package control and search for themes. I would recommend using the [Material theme](https://github.com/equinusocio/material-theme) or [Brogrammer Theme](https://github.com/kenwheeler/brogrammer-theme).

