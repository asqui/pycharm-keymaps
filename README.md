# pycharm-keymaps

This is my PyCharm keymap, based on the Default PyCharm keymap.


## Keyboard Shortcuts

A useful printout quick-reference guide to the default keyboard shortcuts:
https://www.jetbrains.com/pycharm/docs/PyCharm_ReferenceCard.pdf

Additional shortcuts in this keymap:

| Shortcut          | Action
| ----------------- | ----------------- 
| Ctrl+Y            | **Redo** (as opposed to Delete Line in the default keymap)
| Shift+Ctrl+D      | **Diff** current file against repo version (i.e. show my local changes)
| Ctrl+Alt+D        | **Diff** clipboard contents with the current selection
| Alt+S, Alt+T      | **Stack Trace Explorer** - display the stack trace from the clipboard with hyperlinks to the code for each frame.
| Ctrl+L            | **Log** - show the git log for this file.
| Shift+Ctrl+L      | **Log for Selection** - show the git history for the currently selected code lines.
| Alt+L             | **Local History Log** - show the local edit history, annotated with versions when tests passed/failed, etc.
| Shift+Alt+L       | **Local History for Selection**
| Ctrl+Alt+Q        | **Annotate**
| Ctrl+F5           | **Rerun** previous configuration (e.g. previous unit test run)
| Ctrl+Shift+F5     | **Rerun Failed Tests**

The following useful shortcuts are actually part of the standard keymap, but not on the reference card linked above!

| Shortcut              | Action
| --------------------- | -----------------
| Alt+J                 | **Spawn multi-cursor** at the next occurrence of the currently selected text.
| Shift+Alt+J	        | **Undo spawn multi-cursor**, if you went too far.
| Ctrl+Alt+Shift+Insert | **Create New Scratch File**
| Ctrl+Shift+E          | **Recent Locations** pop-up -- includes code snippets of previous locations
| Alt+Shift+E           | **Execute selection in console** -- useful to execute snippets of code when debugging.
| Ctrl+Shift+Quote (')  | **Maximize Tool Window** -- useful for seeing long output (e.g. stack traces)


## Usage

To make use of this keymap:

	cd ~/.config/JetBrains/PyCharm2021.3/                      # On Linux
	cd ~/Library/Application Support/JetBrains/PyCharm2021.3/  # On OS X
	git clone https://github.com/asqui/pycharm-keymaps.git keymaps

(If you already have keymaps, you may need to remove `keymaps/`, or move it away and merge it after cloning the repo.)

If you've lost the .git directory in your checkout (sometimes happens with PyCharm upgrades):

	git init
	git remote add origin https://github.com/asqui/pycharm-keymaps.git
	git fetch
	git reset origin/master
