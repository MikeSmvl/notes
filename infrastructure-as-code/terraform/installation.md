# Installation

[Homebrew](https://brew.sh) is a free and open-source package management system for Mac OS X. Install the official [Terraform formula](https://github.com/hashicorp/homebrew-tap) from the terminal.

First, install the HashiCorp tap, a repository of all our Homebrew packages

```
 brew tap hashicorp/tap
```

Now, install Terraform with `hashicorp/tap/terraform`.

```
brew install hashicorp/tap/terraform
```

Install autocompletion

```
terraform -install-autocomplete
```

Update Terraform

```
brew upgrade terraform
```
