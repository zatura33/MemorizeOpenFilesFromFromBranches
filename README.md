# MemorizeOpenFilesFromFromBranches

**What is it for ?**<br>
This extension has been created to save time in support or other development task that requires to change branch oftenly.<br>

**How does this save time ?**<br>
It is keeping in memory the last opened files in your branch from visual studio. When you get back on this branch there
will be a prompt window that ask you if you want to open back the files you use to have last time.
<br><br>
By default the opened files are automatically saved.<br><br>
**Manually**<br>
In this mode you need to use the Take open files snapshot to save opened files.<br>
To recover opened files you need to use get last opened files in branch.<br><br>
![image](https://github.com/zatura33/MemorizeOpenFilesFromFromBranches/assets/19225363/f6fd57d2-b9d8-4c97-8b0e-0141f4979405)
<br>
<br>
**Configuration**<br>
There is a configuration file for the extension located in :  <br>
<table style="overflow: hidden;">
<tr>
    <td>Alias path</td>
    <td>%LocalAppData%\MemorizeOpenFileFromBranches\Extension.cfg</td>
  </tr>
  <tr>
    <td>Real path</td>
    <td>C:\Users\[username]\AppData\Local\MemorizeOpenFileFromBranches\Extension.cfg</td>
  </tr>
  <tr>
</table>
<br>
In this configuration file you are able to setup the way you want to work with MemorizeOpenFilesFromFromBranches Extension.
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

**Configuration definition**
<br>
<table style="overflow: hidden;">
  <tr>
    <td>Setting name</td>
    <td>Type</td>
    <td>Description</td>
  </tr>
    <tr>
    <td>NumberOfParentToFindGit</td>
    <td>Integer</td>
    <td><sup>The number of folder that the extension will climb up from the solution folder to search the .git folder file</sup></td>
  </tr>
  <tr>
    <td>OpenFilesInSecondsInterval</td>
    <td>Integer</td>
    <td><sup>The delay from wich the files and branch change will be checked/saved</sup></td>
  </tr>
  <tr>
    <td>IsManualUse</td>
    <td>Boolean</td>
    <td><sup>If you choose to use the extension manually.</sup></td>
  </tr>
 <tr>
    <td>NoBranchChangePopUp</td>
    <td>Boolean</td>
    <td><sup>A popup that you is shown each time your branches change.</sup></td>
  </tr>
 <tr>
    <td>CloseOldOpenedFilesBeforeOpening</td>
    <td>Boolean</td>
    <td><sup>Close all already opened file before opening last saved files.</sup></td>
  </tr>    
</table>
<span style="color:red"> * Warning there was a trouble in version 1.6 please do not use this version.</span>






