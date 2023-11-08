# Installing macOS

## Fresh Install, Is Best Install

I usually prefer wiping out my whole hard drive and just doing a fresh install. I've done macOS upgrades in the past but I still feel the bloat after two continuous OS upgrades. So let's create a bootable macOS installer!

First, download the latest macOS on the App Store:





<figure><img src="../.gitbook/assets/Screenshot 2023-11-07 at 8.23.31 PM (1).png" alt=""><figcaption><p>Search for macOS Sonoma in your App Store</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot 2023-11-07 at 8.26.38 PM.png" alt=""><figcaption><p>macOS Sonoma currently being downloaded</p></figcaption></figure>

## Creating A Bootable Installer

There are numerous apps and ways to create a bootable macOS install. As of this writing, [Disk Maker X](https://diskmakerx.com/) no longer supports older macOS starting from Big Sur. Fortunately, you can still easily do this on your Terminal. Here's how you create a bootable thumb drive:

* Prepare a 16GB USB thumb drive that's ready to be wiped out
* Make sure you already have downloaded macOS Sonoma. After downloading, It should be sitting in your Applications folder like this:

![You can find it under Applications > Install macOS Sonoma](<../.gitbook/assets/Screen Shot 2022-01-02 at 10.00.20 PM.png>)

* Insert your thumb drive and simply run this command below on your terminal. Make sure you replace "**Untitled"** with the name of your USB thumb drive.

```
sudo '/Applications/Install macOS Sonoma.app/Contents/Resources/createinstallmedia' --volume '/Volumes/Untitled'
```

* Wait for around 10-15 minutes to complete. You should see this after completing it:

<figure><img src="../.gitbook/assets/Screenshot 2022-12-04 at 4.31.44 AM.png" alt=""><figcaption><p>Bootable macOS Ventura installer completed successfully</p></figcaption></figure>

## Backup Checklist

* [ ] Files on your **Desktop**&#x20;
* [ ] Files in your **Downloads** folder
* [ ] Files in your **Documents** folder
* [ ] Files on the **Pictures** folder&#x20;
* [ ] Code in your **Git** folder
* [ ] Tiny code snippets or links\
  (Instead of saving them on iCloud notes or on Sublime Text or in note-taking apps - use [Paste](https://pasteapp.me/))
* [ ] Browser bookmarks, settings, history, etc.  \
  If you're using different browsers, [Raindrop.io](https://raindrop.io/) is a great bookmark manager.
* [ ] **Passwords**, **server logins** & **sensitive stuff**.\
  Don't store them in your notes. Use password managers like [1Password](https://1password.com/) or [LastPass](https://www.lastpass.com/). I recommend using [Bitwarden](https://bitwarden.com/) — the free tier is good enough for my personal needs and is open-source.
* [ ] Don't forget to backup your public SSH keys too
* [ ] Your saved **Font Files**

## Cloud Storage

Before, I used to back everything up to an external hard drive. Now, I sync all my files to the cloud. [Dropbox](https://www.dropbox.com/) is great (And right-clicking to share public links works like a charm). But I see [Google One ](https://one.google.com/)as a more economically viable option. And if you're living in an Apple ecosystem, [iCloud](https://www.apple.com/ph/icloud/) might make more sense for you.

{% tabs %}
{% tab title="Google One" %}
<figure><img src="../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Apple iCloud" %}
<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Dropbox" %}
<figure><img src="../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}

## Let The Purge Begin

Now it's time to take a deep breath, shutdown your machine, and hope there won't be an ounce of regret. 🐵

{% hint style="warning" %}
**Warning** There's no going back after this point, so be sure to backup your files to the cloud. And if you don't feel comfortable with it, just do a manual backup using your external hard drive.
{% endhint %}

Insert the bootable USB and upon pressing the power key, **hold the option key** until it loads up a screen which prompts you to choose which device you want to boot from. So select the thumb drive with the macOS installer.

![](<../.gitbook/assets/image (16).png>)

Select **Disk Utility** and click **Continue**.&#x20;

![](<../.gitbook/assets/image (17).png>)

Currently what you see here are the drive partitions. What we want to do is to wipe up the whole hard drive. Select **View** > **Show All Devices**

Then select the physical storage device you want to erase (ex. _APPLE SSD AP0512J Media_), then click **Erase**

Select **GUID Partition Map** and **Apple File System (APFS)** for the file system format. Then enter a name.

After that, go back and click on **Reinstall OS X**.

The process is pretty much straightforward into a series of clicking **next**.
