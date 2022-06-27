---
id: 3bfxdktw3xb16gdyxiqw2vk
title: Root
desc: ''
updated: 1656304754822
created: 1655788389561
---
## Root

[[fe]]
[[proto]]
[[lang]]

## Lookup

This section contains useful links to related resources.

- <https://www.kevinslin.com/notes/3dd58f62-fee5-4f93-b9f1-b0f0f59a9b64/>
- [Getting Started Guide](https://link.dendron.so/6b25)
- [Discord](https://link.dendron.so/6b23)
- [Home Page](https://wiki.dendron.so/)
- [Github](https://link.dendron.so/6b24)
- [Developer Docs](https://docs.dendron.so/)

## Table of Contents

<!-- Amoeba Structure Flat Hiearchy -->

- [Root](#root)
- [Lookup](#lookup)
- [Table of Contents](#table-of-contents)
- [Journal](#journal)
- [Git](#git)
  - [Branches](#branches)
    - [Renaming branches](#renaming-branches)
  - [Troubleshooting](#troubleshooting)
    - [Reference errors](#reference-errors)
- [Concepts](#concepts)
  - [NLP](#nlp)
    - [Natural Language Processing](#natural-language-processing)
      - [Rust](#rust)
        - [Crates](#crates)
      - [Node](#node)
        - [NPM](#npm)
- [REGEX](#regex)
  - [Resources](#resources)
- [Package Managers](#package-managers)
  - [Node Modules](#node-modules)
  - [Cargo](#cargo)

## Journal

- [[root.journal.2022.06.23]]
  - Run rust functions in JavaScript with node.js by Chris Hay

## Git

### Branches

#### Renaming branches

- Renaming the Local master Branch to main
  - The first step is to rename the "master" branch in your local Git repositories:
  `$ git branch -m master main`

### Troubleshooting

#### Reference errors

-
- git pull fails "unable to resolve reference" "unable to update local ref"

  ```shell
  error: update_ref failed for ref 'refs/remotes/origin/main'
  : cannot lock ref 'refs/remotes/origin/main'
  : unable to resolve reference 'refs/remotes/origin/main': reference broken
  ```

  - <https://stackoverflow.com/a/15458951>

  ```shell
  rm .git/refs/remotes/origin/master
  git fetch
  ```

## Concepts

### NLP

#### Natural Language Processing

##### Rust

###### Crates

- [tokenizers](https://crates.io/crates/tokenizers)

##### Node

###### NPM

- [compromise](https://www.npmjs.com/package/compromise)

- FFI (Foreign Function File)
  - <https://stackoverflow.com/a/66479059>
    - Why does npm install ffi return error. Using node version 12
  - For Windows users!
    - If your didn't install node-gyp then visit this link <https://github.com/nodejs/node-gyp#on-windows>
    - Downgrading Node version worked for me.
      - In order to downgrade Node version use NVM For windows
    - On Windows
      - Install the current version of Python from the Microsoft Store package.
  - Install tools and configuration manually:
    - Install Visual C++ Build Environment: Visual Studio Build Tools
    - (using "Visual C++ build tools" workload) or Visual Studio Community
    - (using the "Desktop development with C++" workload)
    - Launch cmd, npm config set msvs_version 2017

## REGEX

### Resources

- RegexOne
  - <https://regexone.com/>
  - Learn Regular Expressions with simple, interactive exercises.

## Package Managers

### Node Modules

- `npx npkill`
  - Delete Node Modules files on system (picker)

### Cargo
