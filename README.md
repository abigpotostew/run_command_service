#Run Shell Command Finder Service v0.6
##By Stewart Bracken
===
####Mac Finder service to quickly run a shell command on selected Finder items

###Installation:
1. Place 'run_command_on_files.workflow' into ~/Libary/Services

###Tips:
* I highly recommend giving this service a keyboard shortcut. You can do this by going to System Preferences > Keyboard > Shortcuts > Services (left box), and finding the run_command_on_files item. Assign your favorite shortcut to this!
![ScreenShot](screenshot.png)


###Usage:
1. Highlight item(s) in Finder.
2. Activate the service: (A) Use your shortcut. or (B) Control click the selection, navigate to Services, and select run_command_on_files.
3. Type in a shell command. Use the operator '@' to insert the filename into the command. Place the double operator, '@@', to insert the full absolute path for the selected file in your shell command. Note that this service sets the working directory to the parent directory of the selection.

======


#####Bugs:
* none that I know of. Please let me know if you find any.

#####Fixed Bugs:
* as of v0.5 file names with spaces don't work. fixed in v0.6
* rm doesn't work. fixed in v0.5

======

###Changelog:
####v0.6
* The script now changes directories into the parent folder of your selected finder item before running the shell command.
* '@' operator changed to inserting the filename + extension of the selected finder item. 
* '@@' operator added which inserts the full absolute path of the selected finder item.

####v0.5
* updated applescript algorithm to a simplified terminal do script process.
* for each selected finder item, a new terminal window opens to easily view script output.
