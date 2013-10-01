### WAPPSCmdlets module
These are the files required to load- and use the WAPPSCmdlets that were previously available at CodePlex.  WAPPSCmdlets were a PowerShell module back in the day (call it late 2011), before Microsoft had an "official" Azure cmdlets release.
Files in this collection that are from the Windows Azure SDK, v1.6, x64:
	- Microsoft.WindowsAzure.Diagnostics.dll
	- Microsoft.WindowsAzure.Diagnostics.xml
	- Microsoft.WindowsAzure.StorageClient.dll
	- Microsoft.WindowsAzure.StorageClient.xml


By having those (along with the items directly below) in the same directory as the WAPPSCmdlets.dll and WAPPSCmdlets.dll-Help.xml files, one can import the WAPPSCmdlets.dll "module" (via something like `Import-Module <pathToTheseFiles>\WAPPSCmdlets.dll`), and the rest of the dependencies are auto-loaded.
	- Microsoft.WindowsAzure.Samples.Management.Service.dll
	- Microsoft.WindowsAzure.Samples.Management.Service.pdb
	- Microsoft.WindowsAzure.Samples.Management.SqlAzure.dll
	- Microsoft.WindowsAzure.Samples.Management.SqlAzure.pdb
	- Microsoft.WindowsAzure.Samples.Management.Storage.dll
	- Microsoft.WindowsAzure.Samples.Management.Storage.pdb
	- Microsoft.WindowsAzure.Samples.Management.TrafficManager.dll
	- Microsoft.WindowsAzure.Samples.Management.TrafficManager.pdb

The other directory ("bak") is of other files that were included originally in the GitHub repo from which this WAPPSCmdlets copy came (https://github.com/RichardSlater/PowershellProfile.git).  They were deemed unnecessary by process of elimination (steps:  left them out of the current directory, tried loading WAPPSCmdlets.dll, resolved "missing" items one at a time, and these are the files that were never requested in the load process)
