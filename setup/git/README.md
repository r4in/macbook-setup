# Git

What's a developer without [Git](http://git-scm.com/)? To install, simply run:

```text
brew install git
```

When done, to test that it installed fine you can run:

```text
git --version
```

And `which git`should output`/usr/local/bin/git`. If not, try restarting the terminal.

Next, we'll define your Git user \(should be the same name and email you use for [GitHub](https://github.com/)\):

```text
git config --global user.name "Your Name Here"
git config --global user.email "your_email@youremail.com"
```

They will get added to your `.gitconfig`  file.

To push code to your GitHub repositories, we're going to use the recommended HTTPS method \(versus SSH\). So you don't have to type your username and password every time, let's enable Git password caching as described [here](https://help.github.com/articles/set-up-git):

```text
git config --global credential.helper osxkeychain
```

## SSH Keys <a id="ssh-config-for-github"></a>

You can generate ssh keys for your machine by running

```text
ssh-keygen
```

Then, press enter thrice.

You can checkout your public key by navigating to

```text
cd ~/.ssh
```

Type `ls -a` and you should be seeing **id\_rsa** _****_\(your private key\) and **id\_rsa.pub \(**your public key\)

![](../../.gitbook/assets/image%20%2821%29.png)

Then type `cat id_rsa.pub` to see your public key so you could copy paste it to your Github/Bitbucket





