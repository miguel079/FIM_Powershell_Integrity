<h1>Powershell File Integrity Monitor Script Walkthrough</h1>

<h2>Description</h2>
In this lab I show how to create a custom File Integrity Monitor in Powershell with Azure. The script reviews the contents of the Folder titled "Files" and compares the Hashes to determine the file integrity. The script then informs the user if a file has been changed, deleted, or if a new file has been created. In the broader scope of Cyber security, this script focuses on the Integrity aspect of the CIA triad.
<br/>


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Azure Cloud Shell</b>

<h2>Environments Used </h2>

- <b>Powershell Version 7.3.6</b> (21H2)
- <b>Azure Cloud Shell</b>

<h2>Program walk-through:</h2>

<p align="center">

Within the Azure Cloud Powershell Open Editor and Split screen Between the Command Line (Bottom in blue) and Editor (Top):  <br/>
<img src="https://i.imgur.com/dql2gNf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Make sure to create all of the files and folders within the same directory (in this case I have created a directory titled "FIM"). This also shows that I ran the FIM.ps1 script and it has successfully displayed the prompt for the user to start the File Integrity Monitor<br />
<br />

Here we describe the conditional statement that describes the options for the FIM and what to do based on our selection: <br/>
<img src="https://i.imgur.com/KQWtgkM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
The first option, "Option A", collects a new baseline by calculating a hash value and assigns it to each file within the Files directory. It then creates a baseline.txt file to store this information. This particular statement also deletes a pre-existing baseline.txt file if it already exists.
<br />
<br />

The second option, "Option B", monitors files from the saved Baseline and checks against the hash values to make sure the files have not been altered: <br/>
<img src="https://i.imgur.com/uFNKimT_d.webp?maxwidth=1520&fidelity=grand" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Here we see that the script alerts the user if a new file has been created, which can be confirmed by creating a new file and running the script: <br/>
<img src="https://i.imgur.com/DgcHkSp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Here is a demonstration of the script alerting the user to a file being changed: <br/>
<img src="https://i.imgur.com/GvtUjjM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Finally we see an instance where a File has been deleted (this can also be tested by moving the file out of the directory): <br/>
<img src="https://i.imgur.com/4lATC8Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
Side Note: It's important to consider the user's side, which is why each script alert is a different color (a new file is shown as green, a file being changed is yellow, and a deleted file alert is displayed in red with a gray background).
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
