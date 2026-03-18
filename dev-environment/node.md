# Node

Node.js lets you run JavaScript on your computer instead of just in a browser. It’s used to build backend services, run development tools, and manage packages (via npm) for modern apps.

#### Node Version Manager

nvm (Node Version Manager) is a tool that lets you install and switch between different versions of Node.js on your computer.

To install, run:

```zsh
brew install nvm
```

Then create the nvm folder:

```zsh
mkdir ~/.nvm
```

Then add this to your .zshrc configuration file

```
export NVM_DIR="$HOME/.nvm"
[ -s "$(brew --prefix nvm)/nvm.sh" ] && \. "$(brew --prefix nvm)/nvm.sh"
```

Then reload your config

```
source ~/.zshrc
```

#### Node

Then install the LTS (Long-Term Support) version. This means a stable, well-tested version of software that gets updates and fixes for a long time.

```zsh
nvm install --lts
```

#### npm

npm (Node Package Manager) is a tool that lets you install and manage libraries (packages) for your JavaScript projects. This comes bundled with Node.js which we have previously installed.

You can verify that npm was installed by typing:

```zsh
npm --version
```
