# git-setup
Git commands to setup your development environment

## Basics

Set your name
```
git config --global user.name "Your name"
```

Set your email
```
git config --global user.email "Your email"
```

## Signing commits using your GPG key (Windows)

### Prerequisites

You have
* A GPG key pair created
* Gpg4win installed

Set your GPG key
```
git config --global user.signingkey "Your 32-bit GPG key fingerprint"
```

Sign every commit from now on
```
git config --global commit.gpgsign true
```

Set location of Gpg4win
```
git config --global gpg.program "C:/Program Files (x86)/GNU/GnuPG/gpg2.exe"
```

Finally, add your GPG key to your GitHub account [here](https://github.com/settings/keys).