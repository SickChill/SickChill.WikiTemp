## What is Post Processing?

Post Processing is a name for a collection of actions that are taken after a file is downloaded. You can think of moving the file, renaming or any other process you prefer.

## Post Processing Explained

To start Post Processing in SickChill you have 3 possibilities. The fist (default) one is to let SickChill scan/monitor the `TV Download Dir` for newly downloaded episodes by your download client. Once SickChill detects a new file the Post processing starts. The second possibility is [Manual Post Processing](Post-Processing#manual-post-processing). The third method is using a script to inform SickChill that a new episode was downloaded. This is the ideal/preferred way for NAS devices. As this method doesn't need the constant scanning of the `TV Download Dir` it will allow the hard disks to go into sleep. Some might already be familiar with the SABtoSickbeard script that is used in combination with SABNZBz. However not all download clients support the running of those scripts after a download so SickChill can be informed.  
For more detailed information about an individual setting see the [Main Settings Wiki](Settings-explained#post-processing).

## Manual Post Processing

Normally SickChill does Auto Post Processing, but it gives you also the possibility to Manual Post Process files. This can be handy if you have manually downloaded files and want to instantly process them in SickChill. Simply hit the button Post-Processing in the top-right corner and the following screen will appear.:

![pp](images/postprocess.png)

`Enter the folder containing the episode:`  
Browse to the folder you want to Post-Process.  
`Process Method to be used:`  
Lets you set the method for post-processing, you have the following options.

- `Copy`  
  Copy's the file to your show folder. (And so leaves a copy in your `TV Download Dir` present)
- `Move`  
  Moves the file to your show folder. (And so removes the file in your `TV Download Dir`) You cant use this if you are seeding the file.!
- `Hard link`  
  Creates a hard link in your shows folder, and leaves the file also in your `TV Download Dir`. This is ideal if you want to seed your file. Once you are done seeding simply let the download client remove the file.
- `Symbolic link`  
  Creates a link in your shows folder to the file inside your `TV Download Dir`. Note if you remove the file the link also doesn't work anymore.!

`Force already Post Processed Dir/Files:`  
Forces already Post Processed Dir/Files, use only in case you have problems.  
`Mark Dir/Files as priority download:`  
?  
`Delete files and folders:`  
SickChill deletes the files and folders after completion of the manual Post-Processing.  
`Mark download as failed:`  
Lets you mark the downloaded episode as failed, and lets SickChill search/snatch an alternative file.

## Extra Scripts:

Examples:

- Windows: `C:\Python27\pythonw.exe C:\Script\test.py`
- Linux: `python /Script/test.py`

Use single backslashes, SickChill/Python will escape them and make them double.  
Additional scripts can be used, separated by `|`  
Scripts are called after SickChill's own post-processing.

Parameters that are passed:

- argv[0]: File-path to Script
- argv[1]: Final full path to the episode file
- argv[2]: Original full path of the episode file
- argv[3]: Show indexer ID
- argv[4]: Season number
- argv[5]: Episode number
- argv[6]: Episode Air Date
