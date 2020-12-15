# ChoiceScript Save Plugin (Extended)
Adds the ability to export saves from your current platform (eg. PC, Android, et cetera) and import them to other platforms with the ChoiceScript Save Plugin installed. Also includes a feature that allows deleting all saves on the current platform.

This plugin was forked from <a href="https://github.com/CareyJWilliams">CareyJWilliams</a>'s own <a href="https://github.com/ChoicescriptIDE/ChoiceScriptSavePlugin">ChoiceScriptSavePlugin</a>.

## Installation

<a href="https://github.com/ChoicescriptIDE/ChoiceScriptSavePlugin#installation">The instructions for installing the original ChoiceScript Save Plugin</a> also apply here, with a few differences.

First, <a href="https://raw.githubusercontent.com/adigrateles/ChoiceScriptSavePluginExt/master/ChoiceScriptSavePlugin.js">download ChoiceScriptSavePlugin.js here</a>.

Place it in the same directory as your other script files.

Edit your game's index.html to include the line ```<script src="../ChoiceScriptSavePlugin.js"></script>```.

Add a line for ```window.storeName = "(your_game_here)";``` if it doesn't exist already; change ```(your_game_here)``` to a unique name that's not already used by another choicescript game.

## Usage Notes

This plugin includes virtually all of the same features found in <a href="https://github.com/ChoicescriptIDE/ChoiceScriptSavePlugin">the original ChoiceScript Save Plugin</a>. It also adds methods for exporting and importing saves for a given game, as well as methods for deleting all current saves in one go.

### Export / Export All
**Export** takes the save currently selected in the drop-down menu and copies it to a text file. Clicking the 'Export' button will bring up a prompt asking the user to name the file. Press "Confirm" to download the file *(Note: Leaving the input field blank will result in the file using a game and save name identifier.)*.

**Export All** takes all saves listed in the drop-down menu and copies them to a text file, with each save split into separate lines. Clicking the 'Export All' button will bring up a prompt asking the user to name the file. Press "Confirm" to download the file *(Note: Leaving the input field blank will result in the file using a game identifier.)*.

### Import
**Import** takes data given by the user and parses it into save(s) that will appear in the drop-down menu. Clicking the 'Import' button will bring up a prompt with an empty text area; copy the text from your exported file and paste it into the text area. Press "OK" to convert the save(s) *(Note: Multiple saves can be pasted into the text area. Ensure each save is separated into their own line.)*.

### Delete All
**Delete All** deletes all saves listed in the drop-down menu. Clicking the 'Delete All' button will bring up a prompt asking the user to confirm this action. Press "OK" to delete all saves *(Note: Saves will not be retrievable after deletion.)*.

