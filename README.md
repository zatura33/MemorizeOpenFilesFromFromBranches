# MemorizeOpenFilesFromFromBranches

**What is it for ?**<br>
This extension has been created to save time in support or other development task that requires to change branch oftenly.

**How does this save time ?**<br>
It is keeping in memory the last opened files in your branch from visual studio and when you get back on this branch there<br>
is a prompt window that ask you if you want to open back the files you use to have when you where in this branch last time.<br>
<br>
By default the opened files are automatically saved.<br>
<br>
**Manually**<br>
In this mode you need to use the Take open files snapshot to save opened files.<br>
To recover opened files you need to use get last opened files in branch.<br>
![image](https://github.com/zatura33/MemorizeOpenFilesFromFromBranches/assets/19225363/f6fd57d2-b9d8-4c97-8b0e-0141f4979405)
<br>
**Configuration**<br>
There is a configuration file for the extension located in %LocalAppData%\MemorizeOpenFileFromBranches\Extension.cfg<br>
The real path is C:\Users\[username]\AppData\Local\MemorizeOpenFileFromBranches\Extension.cfg<br>
In this configuration file you are able to setupe the way you want to work with MemorizeOpenFilesFromFromBranches Extension.<br>
Here's an example file:<br>
<code>
{
  "NumberOfParentToFindGit": 10,
  "OpenFilesInSecondsInterval": 10,
  "IsManualUse": false,
  "NoBranchChangePopUp": false,
  "CloseOldOpenedFilesBeforeOpening": true
}
</code><br><br>
**Configuration definition:** <br>
1. NumberOfParentToFindGit           -> An integer, it's the number of folder that the extension will climb up from the solution folder to search the .git folder file
2. OpenFilesInSecondsInterval        -> An integer, the delay from wich the files and branch change will be checked/saved
3. IsManualUse                       -> A boolean, If you choose to use the application manually.
4. NoBranchChangePopUp               -> A boolean, A popup that you want to be shown each time your branches change.
5. CloseOldOpenedFilesBeforeOpening  -> A boolean, close all already opened file before opening last saved files. 






