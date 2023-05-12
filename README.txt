
Tool for migrating and converting NetScaler configuration to Enhanced SSL Profile-specific configuration.

Description:
=========
When the default SSL Profile is enabled the in-built default SSL Profile gets attached to SSL entities and the entire SSL configuration changes to DEFAULT settings. This tool will scan the provided NetScaler configuration file and will generate the following commands and write them in a batch file.


Execution:
========
The following command needs to be executed from the client machine where this tool is downloaded. It will generate the batch file having the SSL Profile-specific commands based on the Netscaler configuration. This batch file after evaluation can be batched on NetScaler after enabling the default Profile setting

For Linux
=========
> ./SSLconfigConverter_linux

For Windows
===========
> ./SSLconfigConverter.exe

For Mac
=======
> ./SSLconfigConverter_mac


> 'SSL PROFILE MIGRATION TOOL WILL HELP CONVERT THE LEGACY NETSCALER ' CONFIGURATION TO ENHANCED SSL PROFILE CONFIGURATION') 
                        --> General Information for Admin 

> PROVIDE THE LATEST SAVED NETSCALER CONFIGURATION FILE 
                        --> This is to provide the latest NetScaler configuration file path (ns.conf)

> IF YOU WANT TO PROVIDE THE SSL PROFILE NAME (TYPE YES) OTHERWISE IF YOU WANT TOOL TO GENERATE THE NAME (TYPE NO) 
                        --> 
		       YES : Admin  to provide name of    SSL Profile
                        NO :  Tool will generate the name of SSL Profile

> The Output Batch File is created  
                       --> This is the batch file with SSL Profile specific commands to be batched later after verifying the batch file and enabling the Default SSL Profile in NetScaler.

> Do you want to review the batch file (Type YES or NO)
                       --> 
			YES : Tool will display the converted SSL Profile commands
                        NO   : Tool will exit and the created batch file can be reviewed later by admin.

Pre-requisites:
===========
> This script can be run from any Linux/Windows/Mac machine having the support of python3
