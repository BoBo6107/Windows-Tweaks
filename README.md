[ReadMe.txt](https://github.com/user-attachments/files/30941019/ReadMe.txt)
~System-Wide Custom Elevated CMD Modification for Windows 10/11~

Author:Fritz

THIS CUSTOM SHORTCUT CAN BE MODIFIED UNDER PROPERTIES TO MEET YOUR NEEDS, AND IT WILL APPEAR ELEVATED WITH YOUR CUSTOMIZATIONS NO MATTER WHERE YOU LAUNCH COMMAND PROMPT FROM.

------------------------------------------------------------
1. REPLACE THE START MENU COMMAND PROMPT SHORTCUT
------------------------------------------------------------

Go to:
C:\Users\YOUR USERNAME\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\System Tools

Find "Command Prompt.lnk".

• Rename the original file to something like "Command Prompt.bak" for safekeeping.
• (Optional) Set the old shortcut to Hidden to reduce clutter.
• Copy the custom "Command Prompt.lnk" from this package into this folder.

This gives you the custom elevated CMD everywhere *except* Win+R.

------------------------------------------------------------
2. PLACE THE .BAT LAUNCHER
------------------------------------------------------------

This package uses the following default path:
C:\Program Files (x86)\customcmd.bat

Place the included .bat file in:
C:\Program Files (x86)\

If you choose a different location, you MUST update the .reg file accordingly or Win+R will not work.

------------------------------------------------------------
3. APPLY THE REGISTRY MODIFICATION (ENABLES WIN+R)
------------------------------------------------------------

Run:
CustomCMD.reg

This creates a new App Paths entry so typing "mycmd" in Win+R launches the custom elevated CMD.

Without running the .reg file, the custom CMD works everywhere EXCEPT Win+R.

If you want Win+R → custom CMD, you MUST run the .reg.

------------------------------------------------------------
4. REVERSAL INSTRUCTIONS
------------------------------------------------------------

To restore the original Start Menu CMD:

Go back to:
C:\Users\YOUR USERNAME\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\System Tools\

• Delete the custom "Command Prompt.lnk".
• Unhide and rename your backup file back to "Command Prompt.lnk".

To restore Win+R behavior:

Run:
Registry Reversal.reg

This removes the custom App Paths entry and returns Win+R to default.

------------------------------------------------------------

-Hope this helps someone-

~Fritz~
