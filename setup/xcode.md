# Xcode

## **Xcode**

Xcode is Apple’s official integrated development environment (IDE) used to build apps for all Apple platforms.

Download and install it from the **App Store** or from [Apple's website](https://developer.apple.com/xcode/).

To verify your installation, run:

```zsh
xcode-select -p
```

And you should see:

```zsh
/Applications/Xcode.app/Contents/Developer
```

Then run:

```zsh
sudo xcodebuild -license accept
```

## Xcode Command Line Tools

Xcode Command Line Tools (CLT) are a lightweight set of developer tools from Apple that let you use programming and build tools without installing the full Xcode app. You'll still need this when installing for Homebrew later on.

To install, run:

```zsh
xcode-select --install
```

