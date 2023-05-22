# Tool to migrate the SSL configuration to the default SSL profile
Tool for migrating and converting the NetScaler SSL configuration to the default SSL profile-specific configuration.

## Description
When you enable the default SSL profile, the in-built default SSL profile is attached to SSL entities and the entire SSL configuration changes to the default settings. As a result, your custom settings are lost. Manually adding the missing entries to the configuration is a tedious task. This tool scans the existing NetScaler configuration file and creates custom profiles. The tool is available for Linux, Windows, and Mac operating systems.

## Prerequisites
The Linux/Windows/Mac device from where this script is run must support Python3. 
You must save the configuration (ns.conf) before running the script.

## Downloads

### For Linux
./SSLconfigConverter_linux

### For Windows
./SSLconfigConverter.exe

### For Mac
./SSLconfigConverter_mac

## Procedure

This script is interactive. When you run the command, some prompts appear. The first prompt is for information purposes only. Second, you are prompted to provide the latest NetScaler configuration file (ns.conf). Third, select YES if you want to provide the SSL profile name. Otherwise, the tool automatically provides a name. The output is a batch file. 

When prompted to review the batch file, type YES to review or NO to exit. Copy the batch file to your NetScaler, enable the default profile, and run the batch command.

The following messages/prompts appear when you run the script:

SSL configuration converter tool helps convert the legacy NetScaler configuration to the default SSL profile configuration

...
>Provide the latest saved NetScaler configuration file (ns.conf):


>Do you want to provide an SSL profile name (Yes/No):
...

(The following prompt appears if you selected YES.)
...
>Type the SSL profile name:
...

A batch file is created.

...
>Do you want to review the batch file (YES/NO):
...
