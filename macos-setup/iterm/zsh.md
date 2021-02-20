# zsh

The Z shell \(also known as `zsh`\) is a Unix shell that is built on top of `bash` \(the default shell for macOS\) with additional features. It's recommended to use `zsh` over `bash`. It's also highly recommended to install a framework with `zsh` as it makes dealing with configuration, plugins and themes a lot nicer.

We've also included an `env.sh` file where we store our aliases, exports, path changes etc. We put this in a separate file to not pollute our main configuration file too much. This file is found in the bottom of this page.

Install `zsh` using Homebrew:

```text
brew install zsh
```

Now you should install a framework, we recommend to use [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh) or [Prezto](https://github.com/sorin-ionescu/prezto). **Note that you should pick one of them, not use both.**

The configuration file for `zsh` is called `.zshrc` and lives in your home folder \(`~/.zshrc`\).

### Oh My Zsh <a id="oh-my-zsh"></a>

[Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh) is an open source, community-driven framework for managing your `zsh` configuration. It comes with a bunch of features out of the box and improves your terminal experience.

Install Oh My Zsh:

```text
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

The installation script should set `zsh` to your default shell, but if it doesn't you can do it manually:

```text
chsh -s $(which zsh)
```

#### Configuration <a id="configuration"></a>

The out-of-the-box configuration is usable but you probably want to customise it to suit your needs. The [Official Wiki](https://github.com/robbyrussell/oh-my-zsh/wiki) contains a lot of useful information if you want to deep dive into what you can do with Oh My Zsh, but we'll cover the basics here.

To apply the changes you make you need to either **start new shell instance** or run:

```text
source ~/.zshrc
```

**Plugins**

Add plugins to your shell by adding the name of the plugin to the `plugin` array in your `.zshrc`.

```text
plugins=(git colored-man-pages colorize pip python brew osx zsh-syntax-highlighting zsh-autosuggestions)
```

You'll find a list of all plugins on the [Oh My Zsh Wiki](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins). Note that adding plugins can cause your shell startup time to increase.

