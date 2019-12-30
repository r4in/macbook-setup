# System Preferences

First thing you should do is update the system. To do that go: **Apple menu \(\) &gt; About This Mac &gt; Software Update.**

Also upgrade your OS in case you want to work on the latest OS. macOS upgrades are usually free so you might as well keep your machine up to date.

If this is a new computer, there are a couple tweaks you could make to the System Preferences.

* [ ] Sign in your Apple ID to sync in your iCloud account

![macOS Catalina System Preferences](../../.gitbook/assets/screenshot-2019-12-30-at-4.47.28-pm.png)

{% hint style="info" %}
These settings below are all optional, consider them suggestions.
{% endhint %}

## General

* [ ] Appearance &gt; Select **Dark**
* [ ] Make sure **Allow Handoff between this Mac and your iCloud devices** is checked

## Dock

* [ ] Size &gt; **Small**
* [ ] Magnification &gt; **Unchecked**
* [ ] Position on screen &gt; **Left**
* [ ] Remove workspace auto-switching by running the following command:

```text
defaults write com.apple.dock workspaces-auto-swoosh -bool NO
```

and then

```text
killall Dock
```

## Internet Accounts

* [ ] Add your Google, Yahoo or iCloud accounts to sync in with the Mail, Calendar, Messages and other macOS apps.

## Users & Groups

* [ ] Set up your Password, Apple ID, Avatar, etc.

## Keyboard

* [ ] **Shortcuts** &gt; **Spotlight** &gt; Unchecked **Show Spotlight search** 

{% hint style="info" %}
Fun fact: **Spotlight** was redesigned completely on [OS X 10.10 Yosemite](https://en.wikipedia.org/wiki/OS_X_Yosemite) and resembles alot to **Alfred.** I still prefer using Alfred over Spotlight for various reasons \(Just do your research\). That being said, we'll be disabling the Spotlight search keyboard shortcut since we'll be using Alfred anyways.
{% endhint %}

## Trackpad

* Point & Click
  * [ ] Check **Tap to click with one finger** 
* Scroll & Zoom
  * [ ] Uncheck all except for **Zoom in and out**

