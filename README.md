# Logseq Privacy Mode plugin


## Overview
A little plugin that offers some privacy options for your Logseq notes. With this plugin, you can easily hide or encrypt specific blocks of text under the blocks with specific tags.

## Usage
The plugin is invoked for the first time using slash commands: "Add private block: encrypt" and "Add private block: hide." These create buttons which, when clicked will toggle the encryption or visibility state of all child blocks. 

You can also change the state with toolbar widgets, but these will affect all items in your graph, not just the individual block. Unlike the embedded buttons, these only do one thing at time, such as decrypt or show all items. What they do (decrypt/encrypt) is defined in the settings.

You can also password lock the decrypt command, but note that the underlying decryption is not (currently) affected by this. The password (set in the settings) only affects the decryption operation, not the actual encryption encoding. This means that your encrypted text can still be decrypted using a base64 decoder even if someone doesn't know the password. (Future versions may add a more secure encryption passphrase, but this isn't currently implemented.) 

Note: be sure to click outside the block you are encrypting or decrypting before running the command.

## Features
### 1. Hide Blocks

Automatically wrap/unwrap children of blocks tagged with `<div>` element. Support for hiding parent block is planned later.

![Alt text](screenshots/demo1.gif)

You could define the tag to mark the blocks to hide as well as style of the hidden test span in the setting.  

### 2. Encrypt Blocks
   
Encrypt/Decrypt blocks with custom tag.

![Alt text](screenshots/demo2.gif)

### 3. Slash Commands

Instead of using global toggles, you could quickly add a block with button to encrypt/decrypt or hide/show the content with the slash commands.

![Alt text](screenshots/demo4.gif)

## Future Enhancement

- Support for hiding parent block.

## License
