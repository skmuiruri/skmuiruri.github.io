---
layout: post
title: Installation and Setup
description: The first post in the Rust programming series. In this post we learn how to install and setup the Rust programming language.
date: 2023-07-14 15:01:35 +0100
author: Samson Kamau Muiruri
image: 'images/rust_series_1.jpg'
tags: [rust]
tags_color: '#618770'
---

# Installation and Setup

### MacOS or Linux

To install Rust in a Mac or Linux station, run the following command in a terminal window

```bash
$ curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
```

This downloads a script and starts the installation of the `rustup` tool. Rustup is the official tool used to manage Rust tooling. It allows you to install Rust, keep it updated, and toggle between stable, beta, and nightly Rust compilers and tooling. 

If the installation is successful, the following line will appear:

`Rust is installed now. Great!`


## Windows

To install Rust in Windows, go to  [https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install) and follow the instructions for installing Rust. 

You will need to install [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/). Select the following workloads when prompted:
- Desktop Development with C++
- The Windows 10 or 11 SDK
- The English language pack component, along with any other language pack of your choosing


To confirm that you've installed Rust correctly, open a shell terminal and run the following command.

```shell
$ rustc --version
```

If you see the version number, commit hash, and commit date for the latest stable version that has been released, then congratulations, you have Rust installed correctly.


## Some Other Useful Commands

The installation process described above installs both the **Rust Compiler (rustc)** and the **Rust package manager (cargo)**.

You can verify their respective versions by running the following commands.

```shell
$ rustc --version 
$ cargo --version
```

You can view the installment paths of the compiler and package manager respectively by running the following commands.

```bash
$ rustup which rustc
$ rustup which cargo
```

You can view the installed toolchains by running the following command

```shell
$ rustup show
```

The `rustup` tool also allows you to maintain installed installed Rust toolchains. Run the following command to check whether new versions exist.

```bash
$ rustup check
```

Run the following command to update to the latest version\.

```bash
$ rustup update
```

You can switch between installed toolchains by simply indicating which version to use. To use the stable simply run the following command

```bash
$ rustup default stable
```

To use the nightly build version run the following command

```bash
$ rustup default nightly
```


## IDE Setting up

### Visual Studio Code
IDE: https://visualstudio.microsoft.com/it/downloads/
Plugin: https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer

### Intelij IDEA
IDE: https://www.jetbrains.com/idea/
Plugin: https://www.jetbrains.com/rust/

