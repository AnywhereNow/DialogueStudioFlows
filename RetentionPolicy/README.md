## Retention Policy
### AnywhereNow Dialogue Studio
## Flow description
Use the Retention Policy Flow to get information from the Retention Policy List in your Sharepoint UCC settings page

The flow will read the list from Sharepoint and use the active settings to read the specific list and delete all entries that are older then the chosen period

![Retention Policy flow](https://github.com/AnywhereNow/DialogueStudioFlows/blob/master/RetentionPolicy\resources/RetentionPolicy.png)

## How to download and import in Anywhere365 Dialogue Studio
- use green download [Code] button, top right from [repository home](https://github.com/Anywhere365/DialogueStudioFlows) or
- click on the .json file, click [raw] on top right, then ctl-A, ctl-C
- Goto hamburger menu, top right, in Dialogue Studio
- Choose Import, then ctl-V or select local file

## Requirements
- You need to enable activate the settings in the RetentionPolicy list on your Sharepoint ucc settings page
- an appid and secret in your Azure is needed with the Sites.ReadWrite.All rights

## Todo after Import
- Change all information in the "required information" function node


## Important to know 
- in Azure you can also use the specific ReadWrite right and add the specific Sharepoint pages to this user



