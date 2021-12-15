- [Introduction](#introduction)
- [Screenshots](#screenshots)
- [Installation](#installation)

## Introduction

> **Note:** This repository is outdated and may not work properly. Please consider opening a pull request or an issue,
> if would like to speed up development of this repository.

A [ZI](https://github.com/z-shell/zi) Annex (i.e. an extension) that automatically generates:

- man pages for all plugins and snippets (out of plugin README.md files by
  using [ronn](https://github.com/rtomayko/ronn) converter),
- code-documentation manpages (by using
  [zsdoc](https://github.com/z-shell/zsdoc) project).

Man extension is being activated at clone of a plugin and also at update of it
and it then generates the manpages. To view them there's a `zman` command:

```zsh
# View README.md manpage in the terminal
zman z-a-man
# View the code documentation (via the full plugin name, as demonstrated)
zman -c z-shell/z-a-man
```

## Screenshots

Main manual (of the project):

![README](https://raw.githubusercontent.com/z-shell/z-a-man/main/docs/images/zman-readme.png)

Code documentation for the plugin.zsh file (of the project):

![Code documentation](https://raw.githubusercontent.com/z-shell/z-a-man/main/docs/images/zman-cd.png)

## Installation

Simply load as a plugin. This will install the extension within [ZI](https://github.com/z-shell/zi):

```zsh
zi light z-shell/z-a-man
```
