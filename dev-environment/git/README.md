# Git

What's a developer without [Git](http://git-scm.com/)? To install, simply run:

```
brew install git
```

When you’re done, run this to confirm it installed correctly:

```
git --version
```

And `which git` should output `/usr/local/bin/git`. If not, try restarting Terminal.

Next, we'll define your Git user (should be the same name and email you use for [GitHub](https://github.com/)):

```
git config --global user.name "Your Name Here"
git config --global user.email "your_email@youremail.com"
```

They will get added to your `.gitconfig` file.

To push code to your GitHub repositories, we're going to use the recommended HTTPS method (versus SSH). So you don't have to type your username and password every time, let's enable Git password caching as described [here](https://help.github.com/articles/set-up-git):

```
git config --global credential.helper osxkeychain
```

## SSH Keys <a href="#ssh-config-for-github" id="ssh-config-for-github"></a>

You can generate SSH keys for your machine by running:

```
ssh-keygen
```

Then press **Enter** three times.

You can check out your public key by navigating to:

```
cd ~/.ssh
```

Type `ls -a` and you should see **id\_rsa** (your private key) and **id\_rsa.pub** (your public key).

![](<../../.gitbook/assets/image (22).png>)

Then type `cat id_rsa.pub` to print your public key, so you can copy-paste it to GitHub/Bitbucket.
