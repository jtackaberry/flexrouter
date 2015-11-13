# FlexRouter

## What is it?

FlexRouter is a highly customizable Kontakt Multiscript designed for managing and unifying keyswitches.  Some features include:

* support for note or CC-based keyswitches
* arbitrary translation between notes and CCs
* can route events to instruments on ports A-D (64 separate channels)
* multiple note-based keyswitches can be activated simultaneously (useful for e.g. layering articulations)
* one instance of FlexRouter supports 16 rules
* each rule supports up to 128 independently configured keyswitches
* probably a few bugs :)

Since a picture is worth a thousand words:

![](https://www.urandom.ca/flexrouter/flexrouter.png)


Here are a few use-cases that can be solved using FlexRouter:

* Put each articulation patch on different channels (up to 64) and control with keyswitches
  from a single channel
* Assign different instruments on channels 1 through 16, each with multiple patches for articulations, and
  control each instrument independently
* Use UACC to control conventional note-keyswitched libraries
* Use UACC with Spitfire libraries, but cherry-pick certain articulations from
  other libraries on other channels
* Notes on channel 16 redirect to Spitfire UACC events on channel 1



## How do I install it?

Follow these steps:

1. Download the [latest compiled script](https://github.com/jtackaberry/flexrouter/releases/latest)
2. Copy the contents to clipboard
3. In your Kontakt instance, click the script button in the toolbar to open the multiscript pane
4. Select the desired slot for the script, and click the edit button
5. Paste the clipboard contents into the newly opened text area
6. Click the Apply button
7. Click the Edit button again to close the edit text area



## How do I contribute or make my own customizations?

### Reporting bugs

Create an account on GitHub and [open an issue](https://github.com/jtackaberry/flexrouter/issues).


### Hacking code

First download and install [Sublime Text 3](http://www.sublimetext.com/3), and then download and install Nils Liberg's excellent [SublimeKSP](http://nilsliberg.se/ksp/) plugin for ST3.

While you're there, click the donate button and buy Nils a coffee for his efforts because there's no way I'd have avoided gouging out my eyes at the abomination that is KSP were it not for Nils' KSP extensions.

Clone this repository, and open the KSP scripts under src/ within ST3.

Use SublimeKSP to compile flexrouter.ksp (see SublimeKSP's README.md for details) and paste the contents of the clipboard (which gets automagically populated by SublimeKSP) into Kontakt as per the installations steps above.

If you want to contribute changes back to FlexRouter, please use the usual GitHub workflow: fork this repository and send me a pull request.  Please don't be offended by scrutiny and nitpicking on any contributed code. :)
