# Git and GitHub {#git-and-github}

What's a developer without [Git](http://git-scm.com/)? To install, simply run:

```
$ brew install git
```

When done, to test that it installed fine you can run:

```
$ git --version
```

And`$ which git`should output`/usr/local/bin/git`.

Next, we'll define your Git user \(should be the same name and email you use for [GitHub](https://github.com/)\):

```
$ git config --global user.name "Your Name Here"
$ git config --global user.email "your_email@youremail.com"
```

They will get added to your`.gitconfig`file.

To push code to your GitHub repositories, we're going to use the recommended HTTPS method \(versus SSH\). So you don't have to type your username and password everytime, let's enable Git password caching as described [here](https://help.github.com/articles/set-up-git):

```
$ git config --global credential.helper osxkeychain
```

### SSH Keys {#ssh-config-for-github}

You can generate ssh keys for your machine by running

```
$ ssh-keygen
```

You can checkout your public key by navigating to

```
$ cd ~/.ssh
```

And you should be seeing **idr**_**sa **_\(your private key\) and **id\_rsa.pub **your public key.

