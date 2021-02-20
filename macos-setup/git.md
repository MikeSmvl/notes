---
description: >-
  Git is a free and open source distributed version control system designed to
  handle everything from small to very large projects with speed and efficiency.
---

# Git

Install using Brew:

```text
brew install git
```

When done, to test that it installed properly you can run:

```text
git --version
```

And `which git` should output `/usr/local/bin/git`.

Next, you can define your global Git user:

```text
git config --global user.name "Your Name Here"
git config --global user.email "your_email@youremail.com"
```

They will get added to your `.gitconfig` file found in the home folder `~/`.

