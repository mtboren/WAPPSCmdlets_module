from the Windows Azure SDK, v1.6, x64:
Microsoft.WindowsAzure.Diagnostics.dll
Microsoft.WindowsAzure.Diagnostics.xml
Microsoft.WindowsAzure.StorageClient.dll
Microsoft.WindowsAzure.StorageClient.xml


By having those (along with the items directly below) in the same directory as the WAPPSCmdlets.dll and WAPPSCmdlets.dll-Help.xml files, can just import the WAPPSCmdlets.dll "module", and the rest of the dependencies are auto-loaded.  The other directory is of other files that were included originally in the GitHub repo from which this WAPPSCmdlets copy came (https://github.com/RichardSlater/PowershellProfile.git)
Microsoft.WindowsAzure.Samples.Management.Service.dll
Microsoft.WindowsAzure.Samples.Management.Service.pdb
Microsoft.WindowsAzure.Samples.Management.SqlAzure.dll
Microsoft.WindowsAzure.Samples.Management.SqlAzure.pdb
Microsoft.WindowsAzure.Samples.Management.Storage.dll
Microsoft.WindowsAzure.Samples.Management.Storage.pdb
Microsoft.WindowsAzure.Samples.Management.TrafficManager.dll
Microsoft.WindowsAzure.Samples.Management.TrafficManager.pdb