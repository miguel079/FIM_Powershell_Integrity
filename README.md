<h1>Powershell File Integrity Monitor Script Walkthrough</h1>

<h2>Description</h2>
In this lab I show how to create a custom File Integrity Monitor in Powershell with Azure. The script reviews the contents of the Folder titled "Files" and compares the Hashes to determine the file inegrity. The script then informs the user if a file has been changed, deleted, or if a new file has been created.
<br/>


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Azure Cloud Shell</b>

<h2>Environments Used </h2>

- <b>Powershell Version 7.3.6</b> (21H2)
- <b>Azure Cloud Shell</b>

<h2>Program walk-through:</h2>

<p align="center">

Within the Azure Cloud Powershell Open Editor and Split screen Between Command Line (on the Bottom and Editor (Top):  <br/>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />

Download Windows 2019 Server: <br/>
<img src="https://i.imgur.com/IJH3PFm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Download Windows 2019 Server: <br/>
<img src="https://i.imgur.com/IJH3PFm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Configure Virtual Box with Windows10: <br/>
<img src="https://i.imgur.com/NtnmZKD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Add Windows 2019 Server: <br/>
<img src="https://i.imgur.com/qb2JZ54.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Assign Password to Default Administrator Account after Installing Windows10: <br/>
<img src="https://i.imgur.com/st3u7kg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Creating Users with <a href="https://github.com/joshmadakor1/AD_PS">Josh Madakor's PowerShell custom script</a>
<img src="https://i.imgur.com/tOmVEhh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
