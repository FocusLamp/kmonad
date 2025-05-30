<h1 align="center">
 <img alt="KMonad" title="KMonad" height="32" src="kmonad.svg"/>
</h1>

<h4 align="center">The Onion of Keyboard Management Tools, available on GNU/Linux, Windows, and MacOS!</h4>

<p align="center">
    <a href="#features">Features</a> •
    <a href="#installation">Installation</a> •
    <a href="#configuration">Configuration</a> •
    <a href="#troubleshooting">Troubleshooting</a> •
    <a href="#disclaimer">Disclaimer</a>
</p>

---

# Running The Colemak-DH + EXTEND layer
### First make sure to add the keyboard event from `/dev/input/event<number>`

Example:
`input  (device-file "/dev/input/event3")`

**to run the layout on Linux**:  `sudo kmonad Colemak-DH-EXTEND.kbd`

---
## Introduction

KMonad is an advanced tool that lets you infinitely customize and extend the functionalities of almost any keyboard. For a detailed list of features, see [here](#features).

If you want to get started with the latest, stable binary release, please check out the master branch, if you are interested in the latest additions and tweaks, switch on over to develop and compile your own binary.

Additionally, if you need any help or just want to say hi,
you can join our [Matrix space](https://matrix.to/#/#Kmonad:matrix.org) or
jump into our [IRC channel](https://web.libera.chat/#kmonad).
There is also a [KMonad Subreddit](https://www.reddit.com/r/Kmonad/).

## Features


KMonad offers advanced customization features such as **layers**, **multi-tap**, **tap-hold**, and much more. These features are usually available at the hardware level on the QMK-firmware enabled keyboards. However, KMonad allows you to enjoy such features in virtually any keyboard by low-level system manipulations.

For a good introduction to KMonad, have a look at [this YouTube video](https://www.youtube.com/watch?v=Dhj1eauljwU).



#### Key Customizations

KMonad lets you map any keyboard button to any keymap. Want to swap the useless **Caps Lock** key with the **Escape** key? Want to have your modifiers such as **Shift** and **Control** on your home row, without breaking your normal typing flow? Want a modifier that is combination of **Alt + Ctrl + Super + Shift**? You can do all of those and much more!

#### Layers

A layer is a set of keymaps assigned to your keyboard's buttons. You can have as many layers on top of your base layer as you want. For instance, you can have your regular QWERTY layout, a Colemak/Dvorak layout, a numbers and symbols layer, a function keys layer, a layer for mouse navigation and system controls --- all in a 60% keyboard. When a particular layer is active, any keypress is interpreted according to the layout defined in that layer. With proper configurations, you can jump to a specific layer or switch to one for the next keypress, or do various other complex manipulations.

#### Multi-Use and Multi-Tap Buttons

Multi-Use Buttons are one of the distinguishing features of KMonad. You can have a single button do different things based on whether it is pressed quickly in succession, or pressed once, or held. For example, you can configure the **Caps Lock** key to act as an **Escape** button when pressed once and released, a **Ctrl** modifier when held-down, and a button to jump to a layer when pressed twice quickly in succession. You can make the left and right **Shift** keys to act like left and right parentheses (like the Space Cadet Shift keys) when tapped once, and regular **Shift** keys when held down. The possibilities are infinite!

#### Command Buttons

With Command Buttons you can trigger shell commands with a tap of any button.

#### And More!

There are many more exciting features of KMonad that you can find in the [configuration tutorial](keymap/tutorial.kbd).


## Installation
For more information on how to install KMonad, please refer to:
- [installation](doc/installation.md)

## Configuration

For information on how to configure KMonad, please refer you to:
- [the configuration tutorial](keymap/tutorial.kbd)
- [quick reference](doc/quick-reference.md)
- [user configurations](https://github.com/kmonad/kmonad-contrib)

Want to add your own keyboard configuration to [kmonad-contrib]? Just
fork the repository, create a new subdirectory using your GitHub
username and submit a pull request!

[kmonad-contrib]: https://github.com/kmonad/kmonad-contrib

### Editor Support for the Configuration Language
- [Emacs](https://github.com/kmonad/kbd-mode)
- [Vim](https://github.com/kmonad/kmonad-vim)
- [VSCode](https://github.com/canadaduane/vscode-kmonad)

### Startup
- There are startup scripts available for different init systems in [`startup/`](startup/).
- A [GNOME Shell extension](https://extensions.gnome.org/extension/6069/kmonad-toggle/)
  is available.

## Troubleshooting
For several commonly asked questions regarding various configuration issues, please see:
- [the FAQ](doc/faq.md)

## Disclaimer
The core maintainer is currently chronically ill with debilitating autoimmune
symptoms. They come and go, but when they are there they very much get in the
way of concentrated work. It is very much his intent to keep working on KMonad
until it is very, very good. But please be aware that he might be gone for weeks
on end, not out of a lack of interest, but out of a lack of capacity. You are
always free to reach out to him by email.
