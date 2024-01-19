# 📃How to PowerShell📃

## Kill a process in PowerShell instead of Task Manager: 
Type the command get-process to get all the process running on your computer, you will get Handles NPM(K) PM(K) WS(K) VM(M) CPU(s) Id ProcessName. Once the Process ID has been identified, you can kill the errant process by entering:             **stop-process -id (Id)**

## How to check if an AD account is locked out:
You can use the following on a domain controller to check the properties of a user account:    **get-aduser -identity testuser -properties**

## How to ping IP address and find out corresponding IP address domain name system (DNS) record:
Type **“ping”** hit space and type the IP address you'd like to ping (e.g., 192.XXX.X.X),and for the Type **nslookup** and the command will return the A record for the domain you ran a query for. You can also type **nslookup** and a ip number ( e.g., nslookup 192.XXX.X.X) the command prompt will return the DNS name and the IP you entered.

## How to save your PowerShell output to a raw text file:
Out-File is the cmdlet you’re looking for.
To use the Out-File cmdlet, you can either use the piping operator to pass output to it or the **-InputObject** parameter to specify the objects to be written to the file.
**Get-Process | Out-File C:\Temp\processes.txt**
Or:
**$proc = Get-Process**
**Out-File C:\Temp\processes.txt -InputObject $proc**
These commands provide the same results, creating a text file containing the output of the Get-Process cmdlet. It’s important to note that the information in the text file will be formatted as if sent to the terminal window.





## How To Run A PowerShell Script
There are two main ways to make a PowerShell script:
The first, which will be familiar if you’ve used Windows Command Line before, is to write scripts directly in notepad. For example, open a new notepad file, and write:

**Write-Host “Hello World!”**

Then save this file as FirstScript.ps1

You can call the script from PowerShell using the command:

& "**X:\FirstScript.ps1**"

And you’ll see the output in PowerShell.

The second, much more powerful way of making PowerShell scripts is to use the Windows PowerShell Integrated Scripting Environment (ISE). With ISE, you can run scripts and debug them in a GUI environment. 
