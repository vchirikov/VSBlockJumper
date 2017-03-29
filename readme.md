# VSBlockJumper

 VSBlockJumper is an extension for Visual Studio that enables vertical navigation between and over blocks of code

![Demo](./media/demo.gif?raw=true "Demo")


# Usage

Jumping takes you outside of the nearest block edge (i.e. the whitespace line adjacent to a block). The only exception is when the cursor reaches BOF or EOF, in which case we jump to the start of the first or last line (respectively).

## Commands

Due to existing keybindings within visual studio (and common extensions like resharper or visual assist), I was unable to implement intuitive default keybindings. I've listed what I wanted to use instead here, and encourage you to manually change your keybindings to those.

|        Command        |  Description                                               | Keybinding (Default)       | Keybinding (Ideal) |
|:--------------------- |:---------------------------------------------------------- |:-------------------------- |:------------------ |
| `Edit.JumpUp`         | Jump to the closest block edge above the cursor            | `Alt+NumpadSubtract`       | `Ctrl+Up`          |
| `Edit.JumpDown`       | Jump to the closest block edge below the cursor            | `Alt+NumpadAdd`            | `Ctrl+Down`        |
| `Edit.JumpSelectUp`   | Jump Up and add the jumped block to the active selection   | `Shift+Alt+NumpadSubtract` | `Ctrl+Shift+Up`    |
| `Edit.JumpSelectDown` | Jump Down and add the jumped block to the active selection | `Shift+Alt+NumpadAdd`      | `Ctrl+Shift+Down`  |


# Credits and Thanks

* [Casey Muratory](https://twitter.com/cmuratori) - I first saw this method for navigating code in his Handmade Hero video series
* [Space Block Jumper](https://marketplace.visualstudio.com/items?itemName=jmfirth.vsc-space-block-jumper) - I use this extension for the same purpose as VSBlockJumper in VSCode
* [Anthony Reddan](https://twitter.com/AnthonyReddan) - That's me!