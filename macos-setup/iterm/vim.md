---
description: >-
  Vim is a highly configurable text editor built to make creating and changing
  any kind of text very efficient. It is included as "vi" with most UNIX systems
  and with Apple macOS.
---

# VIM

### Installation <a id="installation"></a>

To install the latest version, use homebrew:

```text
brew install vim
```

### The Ultimate vimrc <a id="the-ultimate-vimrc"></a>

[The Ultimate vimrc](https://github.com/amix/vimrc) it's a collection of vimrc configurations to make easy the usage of vim.

To download the The Ultimate vimrc, you need to install the git client. If you need install it, use home brew:

```text
brew install git
```

Now, download the vimrc files:

```text
git clone https://github.com/amix/vimrc.git ~/.vim_runtime
```

To install the complete version, run:

```text
sh ~/.vim_runtime/install_awesome_vimrc.sh
```

To install the _basic_ version, run:

```text
sh ~/.vim_runtime/install_basic_vimrc.sh
```

#### Update <a id="update"></a>

To update the vimrc scripts, run:

```text
cd ~/.vim_runtime && git pull --rebase && cd -
```

### Maximum Awesome <a id="maximum-awesome"></a>

[Maximum Awesome](https://github.com/square/maximum-awesome) it's a collection of vim configuration and plugins, like a configuration manager for the vim environment.

#### Installation <a id="installation"></a>

To install it, just make a clone of the repository with the git client:

```text
git clone https://github.com/square/maximum-awesome.git
```

Then install it:

```text
cd maximum-awesome
rake
```

> **NOTE:** the rake command will install all dependencies needed.

