A short Powershell script to set the direction of the reading order for the list.

 

You can choose between:

ltr - left to right

rtl - right to left

none 

 

 

 

It requires installed  SharePoint Online SDK

You have to enter the list information before running the script:

 

 

PowerShell
# Paths to SDK. Please verify location on your computer. 
Add-Type -Path "c:\Program Files\Common Files\microsoft shared\Web Server Extensions\15\ISAPI\Microsoft.SharePoint.Client.dll"  
Add-Type -Path "c:\Program Files\Common Files\microsoft shared\Web Server Extensions\15\ISAPI\Microsoft.SharePoint.Client.Runtime.dll"  
 
# Insert the credentials and the name of the site and list 
$Username="trial@trialtrial123.onmicrosoft.com" 
$AdminPassword="Pass" 
$Url="https://trialtrial123.sharepoint.com/sites/teamsitewithlists" 
$ListName="Generic List" 
$Direction ="none"
$Direction paramater specifies the reading order. Enter "ltr", "rtl" or "none"
 

 

 

 

Related scripts
Set-SPOList properties (module)

Change permission property in lists (article)

Other list-related scripts
