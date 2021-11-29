# vscode config
## Archived and absorbed into https://github.com/jwblangley/dotfiles
Repository to store my vscode settings, keymaps and installed extensions.

## Usage
First install [vscode](https://code.visualstudio.com/)
### Settings and Keymap
Copy the contents of the JSON files to their respective local versions.
### Install extensions
A list of installed extensions is stored in extensions.txt. This can be populated by `code --list-extensions`.

To install these extensions in bulk on a bash terminal run the following: 

    wget -qO- https://raw.githubusercontent.com/jwblangley/vscode-config/master/extensions.txt | while read in; do code --install-extension "$in"; done

Or, for a local file:

    while read in; do code --install-extension "$in"; done < extensions.txt
