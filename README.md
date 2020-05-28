# Service Log On As Inventory Script
 Service Log On As Inventory Script



.SYNOPSIS

Purpose of this script is to report on the accounts that are used to logon as a service.

 

.DESCRIPTION

Script was initially created to analyse what services are logging on as particular service accounts. 

Do not want to report on the built-in principles such as Local Service, Network Service etc.

Want to see explicity set user accounts to for the service. 


.ASSUMPTIONS

Script is being executed with sufficient permissions to  access servers specified

You can live with the Write-Host cmdlets :)

You can add your error handling if you need it.  

Can easily output to CSV if needed

Change the OU and domain information to suit your environment
$Computers  = Get-ADComputer -Filter * -SearchBase "OU=Servers,DC=TailspinToys,DC=com"

 

.VERSION

1.0  23-1-2012  Initial release

 

.Author

Rhoderick Milne  Blogs.technet.com/rmilne

 

.Disclaimer

This Sample Code is provided for the purpose of illustration only and is not intended to be used in a production environment. 
THIS SAMPLE CODE AND ANY RELATED INFORMATION ARE PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED,
INCLUDING BUT NOT LIMITED TO THE IMPLIED WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A PARTICULAR PURPOSE. 
We grant You a nonexclusive, royalty-free right to use and modify the Sample Code and to reproduce and distribute the object code form of the Sample Code,
provided that You agree:
(i) to not use Our name, logo, or trademarks to market Your software product in which the Sample Code is embedded;
(ii) to include a valid copyright notice on Your software product in which the Sample Code is embedded; and
(iii) to indemnify, hold harmless, and defend Us and Our suppliers from and against any claims or lawsuits, including attorneys’ fees, that arise or result from the use or distribution of the Sample Code.
Please note: None of the conditions outlined in the disclaimer above will supercede the terms and conditions contained within the Premier Customer Services Description.
This posting is provided "AS IS" with no warranties, and confers no rights.

Use of included script samples are subject to the terms specified at http://www.microsoft.com/info/cpyright.htm.

