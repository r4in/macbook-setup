# Git

Git is a version control system — it tracks changes in your code and lets you collaborate safely.

To install:

```zsh
brew install git
```

Then verify if it installed correctly:

```zsh
git --version
```

#### Set Identity

Set your name and email so Git knows who is making changes. Use the same name and email as your GitHub account so your commits are properly linked.

```
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

These will get added to your `.gitconfig` file.

## SSH Keys <a href="#ssh-config-for-github" id="ssh-config-for-github"></a>

You can generate SSH keys for your machine by running:

```zsh
ssh-keygen
```

Then press **Enter** three times.

Navigate to:

```zsh
cd ~/.ssh
```

Type `ls -a` and you should your private key and public key

<figure><img src="../../.gitbook/assets/image (54).png" alt="" width="563"><figcaption></figcaption></figure>

Then type `cat id_ed25519.pub` to print your public key, so you can copy-paste it to GitHub/Bitbucket.



