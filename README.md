# d8.dev

## Overview

This is our Drupal 8 playground for our developers.

-----

## Git Flow

This project makes use of the [git-flow](http://nvie.com/posts/a-successful-git-branching-model/) branching model. Please make sure you are familiar with __git-flow__ before you continue work on this project. For the best introduction to getting started with __git-flow__, please read [Jeff Kreeftmeijer's blog post](http://jeffkreeftmeijer.com/2010/why-arent-you-using-git-flow/).

----

### Installing git-flow

#### Mac OS

If you are using a Mac, you should be using [homebrew](http://github.com/mxcl/homebrew) and setup is simple:

```bash
$ brew install git-flow
```

#### Linux

For Linux users, the easiest way to install is using Rick Osborne's __git-flow__ installer script. Run the following command:

```bash
$ wget --no-check-certificate -q -O - https://github.com/nvie/gitflow/raw/develop/contrib/gitflow-installer.sh | sudo bash
```

#### Windows

Please don't do web development on a Windows machine. :)
For help, check out the [git-flow](https://github.com/nvie/gitflow) Github repository for additional instructions.

### Shell Integration

For users of the [Bash](http://www.gnu.org/software/bash/) or [ZSH](http://www.zsh.org/) shells, there is some great work on the [git-flow-completion](http://github.com/bobthecow/git-flow-completion) project by __bobthecow__. It offers tab-completion for all __git-flow__ sub-commands and branch names.


----

## Project Setup

To get started working on __d8.dev__, first clone the development repository:

```bash
$ git clone -b develop git@github.com:augustash/d8.dev.git
```

This will check out the default __develop__ branch. This branch is used for current development and staging environments. To be able to deploy production releases you will need to also have a copy of the __master__ branch on your system. Grab a tracking branch of __master__:

```bash
$ cd d8.dev/
$ git branch --track master origin/master
```

Now that you have a local repository you have to make sure you initialize __git-flow__ as it isn't done for you. Make sure to select the default values at the prompts:

```bash
$ git flow init
```

-----

## Download Drupal and Contrib Files

Although this project has a `settings.php` file in the repo, **we do not put any sensitive information in the file**. All sensitive information or configuration overrides should be created in a `settings.local.php` file. You can either create this file yourself or ask another developer for the distributed version.
