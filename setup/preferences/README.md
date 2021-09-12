# System Preferences

First thing you should do is update the system. To do that go: **Apple menu \(\) &gt; About This Mac &gt; Software Update.**

Also upgrade your OS in case you want to work on the latest OS. macOS upgrades are usually free so you might as well keep your machine up to date.

If this is a new computer, there are a couple tweaks you could make to the System Preferences.

* Sign in your Apple ID to sync in your iCloud account

![Big Sur System Preferences](../../.gitbook/assets/image%20%2812%29.png)

{% hint style="warning" %}
These settings below are all optional, consider them suggestions.
{% endhint %}

## General

* Appearance : **Dark**
* Check **Allow Handoff between this Mac and your iCloud devices**
* Recent Items : **None**

## Dock & Menu Bar

* Size : **Small**
* Uncheck **Magnification**
* Position on screen : **Left**
* Uncheck **Show recent applications in Dock**

### Menu Bar Only

* **Spotlight** &gt; Uncheck **Show in Menu Bar**

Remove workspace auto-switching by running the following command in the terminal:

```text
defaults write com.apple.dock workspaces-auto-swoosh -bool NO
```

and then

```text
killall Dock
```

## Siri

* Uncheck **Enable Ask Siri**

## Internet Accounts

* Add your Google, Yahoo or iCloud accounts to sync in with the Mail, Calendar, Messages and other macOS apps.

## Users & Groups

* Set up your Password, Apple ID, Avatar, etc.

## Keyboard

* **Keyboard &gt;  Press \(Globe Icon\) to** &gt; **Do Nothing**
* **Shortcuts** &gt; **Spotlight** &gt; Unchecked **Show Spotlight search** 
* **Shortcuts** &gt; **Spotlight** &gt; Unchecked **Show Spotlight search** 
* Under **Text**, uncheck the following:
  * Correct spelling automatically
  * Capitalize words automatically
  * Add period with double space

{% hint style="info" %}
Fun fact: **Spotlight** was redesigned completely on [OS X 10.10 Yosemite](https://en.wikipedia.org/wiki/OS_X_Yosemite) and resembles a lot to **Alfred.** I still prefer using **Ueli** over Spotlight for various reasons \(Just do your research\). That being said, we'll be disabling the Spotlight search keyboard shortcut since we'll be using Ueli anyways.
{% endhint %}

## Trackpad

* Point & Click
  * Check **Tap to click**

## Accessibility

* Pointer Control
  * Check **Ignore built-in trackpad when mouse or wireless trackpad is present** \(I only do this when I'm using a wireless mouse\)

