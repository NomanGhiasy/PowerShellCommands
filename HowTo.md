# 📃How to PowerShell📃

## Kill a process in PowerShell instead of Task Manager: 
Type the command get-process to get all the process running on your computer, you will get Handles NPM(K) PM(K) WS(K) VM(M) CPU(s) Id ProcessName. Once the Process ID has been identified, you can kill the errant process by entering:             **stop-process -id (Id)**

## How to check if an AD account is locked out:
You can use the following on a domain controller to check the properties of a user account:    **get-aduser -identity testuser -properties**

## How to ping IP address and find out corresponding IP address domain name system (DNS) record:
Type **“ping”** hit space and type the IP address you'd like to ping (e.g., 192.XXX.X.X),and for the Type **nslookup** and the command will return the A record for the domain you ran a query for. You can also type **nslookup** and a ip number ( e.g., nslookup 192.XXX.X.X) the command prompt will return the DNS name and the IP you entered.

## Out-File
**Need to be fixed/updated** 
