---
description: >-
  Visual Studio Code is a lightweight code editor with support for many
  programming languages through extensions
---

# Visual Studio Code

## Installation

To install the latest version, use Homebrew:

```
brew install --cask visual-studio-code
```

### macOS integration <a href="#macos-integration" id="macos-integration"></a>

Launch VS Code from the [command line](https://code.visualstudio.com/docs/setup/mac#\_launching-from-the-command-line).

After that, you can launch VS Code from your terminal:

* `code .` will open VS Code in the current directory
* `code myfile.txt` will open `myfile.txt` in VS Code

### Useful Extensions <a href="#useful-extensions" id="useful-extensions"></a>

#### Python <a href="#python" id="python"></a>

*   [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) - Python code highlighting

    To enable auto-formatting on "Save", i.e. `⌘ + S`, configure the following:

    1. Change the default formatter to `Black` instead of `Autopep8`. Critical to avoid large diffs. Go to _Preferences_ -> _User Settings_ and update the setting `python.formatter.provider` to `Black`
    2. Enable `Format on Save` Setting: _Editor: Format On Save_ setting on _Code_ -> _Preferences_ -> _Settings_

#### JavaScript <a href="#javascript" id="javascript"></a>

* [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) - Useful to check JavaScript errors and helps in auto-formatting the code
* [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - JavaScript code formatter

#### SQL <a href="#sql" id="sql"></a>

* [PostgreSQL formatter](https://marketplace.visualstudio.com/items?itemName=bradymholt.pgformatter)

#### Markdown <a href="#markdown" id="markdown"></a>

* [Markdown Preview](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced) - Read Markdown files in VSCode

#### GitLens <a href="#gitlens" id="gitlens"></a>

* [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) - Supercharge the Git capabilities built into VSCode

#### Docker <a href="#docker" id="docker"></a>

* [Docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker) - Create, manage, and debug images from within VSCode

#### JSON <a href="#json" id="json"></a>

* [Paste JSON as Code](https://marketplace.visualstudio.com/items?itemName=quicktype.quicktype) - Infers types from sample JSON data, then outputs strongly typed models and serializers for working with that data in your desired programming language
* [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) - Launches a local development server with live reloading for both static and dynamic

#### VS Code Icons <a href="#vs-code-icons" id="vs-code-icons"></a>

* [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons) - Adds unique icons to distinguish different file extensions (easier to glance through your directories)
