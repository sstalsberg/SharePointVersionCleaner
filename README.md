# SharePointVersionCleaner

## Description
The SharePointVersionCleaner script is designed to help manage document versions within SharePoint document libraries. It connects to a specified SharePoint site, iterates through all document libraries, and prunes older versions of files, retaining only a user-defined number of the most recent versions. This script is ideal for SharePoint site administrators looking to optimize storage and maintain version control.

## Requirements
- PowerShell 5.1 or higher
- SharePointPnPPowerShellOnline module
- Access to a SharePoint Online site

## Installation
Before running the script, ensure that the SharePointPnPPowerShellOnline module is installed on your system. If it is not installed, run the following PowerShell command to install it:

```powershell
Install-Module SharePointPnPPowerShellOnline -AllowClobber
```

## Usage
Open PowerShell and navigate to the directory containing the SharePointVersionCleaner.ps1 script.
Run the script using the following command: .\SharePointVersionCleaner.ps1

When prompted, enter the number of latest versions you wish to keep for each document.
Note: The script requires you to log in to your SharePoint site. A web login prompt will appear for authentication.

## Configuration
To target a specific SharePoint site, modify the $SiteURL variable at the beginning of the script with your SharePoint site URL:

```powershell
$SiteURL = "https://yourdomain.sharepoint.com/sites/YourSite"
```
