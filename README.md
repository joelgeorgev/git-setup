# Git Setup

> Git commands to setup your development environment.

## Basics

Set your name

```bash
$ git config --global user.name "Your name"
```

Set your email

```bash
$ git config --global user.email "Your email"
```

Set text editor

```bash
$ git config --global core.editor "vim"
```

## Signing commits using your GPG key (Windows)

### Prerequisites

You have

- A GPG key pair created
- Gpg4win installed

Set your GPG key

```bash
$ git config --global user.signingkey "Your 32-bit GPG key fingerprint"
```

Sign every commit from now on

```bash
$ git config --global commit.gpgsign true
```

Get location of gpg.exe

```bash
$ where gpg
C:\Program Files\Git\usr\bin\gpg.exe
C:\Program Files (x86)\GnuPG\bin\gpg.exe
```

Set location of gpg.exe (Git or GnuPG) in Git config

```bash
$ git config --global gpg.program "C:\Program Files\Git\usr\bin\gpg.exe"
```

Finally, add your GPG key to your GitHub account [here](https://github.com/settings/keys).

### WSL

```bash
$ git config --global gpg.program "/mnt/c/Program Files/Git/usr/bin/gpg.exe"
$ git config --global credential.helper "/mnt/c/Program\ Files/Git/mingw64/bin/git-credential-manager-core.exe"
```
