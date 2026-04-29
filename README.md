# VS-Code Snippets
Since snippets are one of the most useful, time saving features of VSCode, this repository is supposed to enable different people to share their own favorite snippets. 

# Structure
In the main folder, there are three files supposed to be located. First the License file, second the gitignore and lastly a python script, used to copy the snippets into the target folder.

# Desired workflow
Whenever a user needs one of the snippet files, they're supposed to run the python script. The script needs one argument all the time: The desired, relative path to the workspace folder. 
The script looks into the .vscode folder located in the workspace (or creates it if necessary). The optional arguments specify which snippets should be added to the workspace folder. This enables a dynamic reconfiguration of the used snippets.  
Finally there should also be an option to remove the snippet files from the folder with the option clean. This option looks into the folder and removes all the files that also exist in this git repo. 
Ideally the python script also looks into the .gitignore of the workspace (if exists) and adds the vscode snippets there