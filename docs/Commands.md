# Coffer Commands

Below are the commands available to Coffer, and what they do.

### Create

Usage: `coffer create <name>`

Flags: 

`-t` - Create an environment with a template `coffer create <name> -t template.py`

`-v` - Select the version of ubuntu/debian to be installed in an environment `coffer create <name> -v wheezy` NOTE: This flag fails silently, if you insert an invalid version it will default to Ubuntu Precise.

Creates an environment from scratch with the name `<name>`

### Clone

Usage: `coffer clone <name> <clone>`

Creates an exact copy of an environment `<name>` to a new environment by name `<clone>`

### Enter

Usage: `coffer enter <name>`

Flags:

`-c` - Execute a command in your environment as you enter it. `coffer enter <name> -c "cd ~/project;git pull origin master"` NOTE: Unless you put a `/bin/bash` in the command `-c` will not spawn a Bash shell.  

Enters a Coffer environment and launches a Bash shell. 

### List

Usage: `coffer list`

Lists all of the environments available to Coffer.

### Remove

Usage: `coffer remove <name>`

Removes a Coffer environment by name `<name>` 

This is a nonreversible action. Once an environmentis removed, it can not be restored.

### Version

Usage: `coffer version`

Displays the current version of Coffer.

### Rename

Usage: `coffer rename <name> <new name>

Renames an environment
