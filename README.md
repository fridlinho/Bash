For how to enable Fancy Bash

Steps and file fancy-prompts.bash found on https://forums.linuxmint.com/viewtopic.php?t=333591#


STEP 1> Go to your home folder and use ctrl+h to show hidden files

STEP 2> Create a folder with the name ".fancyprompts" without quotes on your home directory.

STEP 3> Copy the file fancy-prompts.bash to that folder that we created now.

STEP 4> Make a backup of the .bashrc file and remember where you kept it.

STEP 5> Open the orginal .bashrc in your home folder in any text editor and scroll to the end and press ENTER twice

STEP 6> Copy the content bellow and paste it and the of the .bashrc file and save it and open your terminal to see if changes were applied.


#:------------------------------------------------------------------------
#:
#: This script cannot be run as a program.  You must source it:
#:
#:     $ bash
#:     $ source fancy-prompts.bash
#:     $ prompt-usage
#:     $ prompt-fancy
#:
#: To install, source this file inside your .bashrc file and set the prompt.
#: If your .bashrc already sets PROMPT_COMMAND then source this file *before*
#: setting PROMPT_COMMAND and have your routine call fancy-prompts-command.
#:
     source ~/.fancyprompts/fancy-prompts.bash
#:    PROMPT_COMMAND=prompt-fancy
     my-prompt-command() {
         ...
         fancy-prompts-command
     }
     prompt-curl -P -p "bash> "
#:
#:------------------------------------------------------------------------
