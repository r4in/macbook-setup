# System Preferences

First thing you should do is update the system. To do that go: **Apple menu \(\) &gt; About This Mac &gt; Software Update.**

Also upgrade your OS in case you want to work on the latest OS. macOS upgrades are usually free so you might as well keep your machine up to date.

If this is a new computer, there are a couple tweaks you could make to the System Preferences.**These settings are all optional, consider them suggestions.**

## General

* Check “Use dark menu bar and dock”

## Users & Groups

* Set up Password, Apple ID, Picture, etc.

## Trackpad

* Point & Click
  * Enable Tap to click with one finger
  * Uncheck three finger drag
* Scroll & Zoom
  * Uncheck all apart from Zoom in and out

## Dock

* Visual settings
  * Change position to left and make the size of Icons small
* Other settings
  * Remove workspace auto-switching by running the following command:

```text
$ defaults write com.apple.dock workspaces-auto-swoosh -bool NO
$ killall Dock
```

## Finder

* General
  * Uncheck everything except "Open folders in tabs instead of new windows"
  * New finder window shows Home directory
* Tags
  * Uncheck everything
* Toolbar
  * Update to add path, new folder and delete
* Sidebar
  * Add home and code directory
  * Remove shared and tags

## Keyboard

* Shortcuts &gt; Spotlight
  * Disable spotlight search by unchecking everything. \(We'll be using Alfred\)

## iCloud

* Add an iCloud account and sync Calendar, Find my mac, Contacts etc.

