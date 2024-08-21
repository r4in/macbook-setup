# Installing macOS

## Fresh Install, Is Best Install

I usually prefer wiping out my whole hard drive and just doing a fresh install. I've done macOS upgrades in the past but I still feel the bloat after two continuous OS upgrades. So, let's create a bootable macOS installer!

First, download the latest macOS on the App Store:





<figure><img src="../.gitbook/assets/Screenshot 2023-11-07 at 8.23.31 PM (1).png" alt=""><figcaption><p>Search for macOS Sonoma in your App Store</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot 2023-11-07 at 8.26.38 PM.png" alt=""><figcaption><p>macOS Sonoma currently being downloaded</p></figcaption></figure>

## Creating A Bootable Installer

There are numerous ways to create a bootable macOS install. As of this writing, [Disk Maker X](https://diskmakerx.com/) no longer supports older macOS starting from Big Sur. Fortunately, you can still easily do this on your Terminal. Here's how you create a bootable thumb drive:

* Prepare a 16GB USB thumb drive that's ready to be wiped out
* Make sure you already have downloaded macOS Sonoma. After downloading, It should be sitting in your Applications folder like this:

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption><p>You can find it under Applications > Install macOS Sonoma</p></figcaption></figure>

* Insert your thumb drive and simply run this command below on your terminal. Make sure you replace "**Untitled"** with the name of your USB thumb drive.

```
sudo '/Applications/Install macOS Sonoma.app/Contents/Resources/createinstallmedia' --volume '/Volumes/Untitled'
```

* Wait for about 10-15 minutes for the process to complete. You should see this once it’s finished:

<figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption><p>Bootable macOS Sonoma installer completed successfully</p></figcaption></figure>

## Backup Checklist

* [ ] Files in your **Desktop** folder
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

I used to back everything up to an external hard drive, but now I sync all my files to the cloud. [Dropbox](https://www.dropbox.com/) is great (and right-clicking to share public links works like a charm). However, I find [Google One](https://one.google.com/about/) to be a more economically viable option. If you’re fully immersed in the Apple ecosystem, [iCloud](https://www.icloud.com/) might make more sense for you.

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

Now it’s time to take a deep breath, shut down your machine, and hope there won’t be an ounce of regret. 🐵

{% hint style="warning" %}
**Warning** here’s no going back after this point, so be sure to back up your files to the cloud. If you’re not comfortable with that, you can always do a manual backup using your external hard drive.
{% endhint %}

Insert the bootable USB, and as you press the power key, hold down the **Option key** until a screen appears prompting you to choose which device you want to boot from. Select the thumb drive with the macOS installer.

![](<../.gitbook/assets/image (16).png>)

Select **Disk Utility** and click **Continue**.&#x20;

![](<../.gitbook/assets/image (17).png>)

What you see here are the drive partitions. Our goal is to wipe the entire hard drive. First, select **View > Show All Devices**. Then, choose the physical storage device you want to erase (e.g., _APPLE SSD AP0512J Media_), and click **Erase**.

Select **GUID Partition Map** and **Apple File System (APFS)** as the file system format, then enter a name for the drive.

Once done, go back and click on **Reinstall OS X**.
