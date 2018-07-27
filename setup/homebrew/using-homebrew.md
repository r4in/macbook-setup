# Usage

To install a package \(or **Formula** in Homebrew vocabulary\) simply type:

```text
$ brew install <formula>
```

To update Homebrew's directory of formulae, run:

```text
$ brew update
```

**Note**: I've seen that command fail sometimes because of a bug. If that ever happens, run the following \(when you have Git installed\):

```text
$ cd /usr/local/Homebrew/
$ git fetch origin
$ git reset --hard origin/master
```

To see if any of your packages need to be updated:

```text
$ brew outdated
```

To update a package:

```text
$ brew upgrade <formula>
```

Homebrew keeps older versions of packages installed, in case you want to roll back. That rarely is necessary, so you can do some cleanup to get rid of those old versions:

```text
$ brew cleanup
```

To see what you have installed \(with their version numbers\):

```text
$ brew list --versions
```

brew 'tree' brew 'speedtest\_cli' brew 'trash' brew 'z'

