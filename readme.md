### WAPPSCmdlets module
These are the files required to load- and use the WAPPSCmdlets that were previously available at CodePlex.  The version that the module reports is '2.2.2.0'.  WAPPSCmdlets were a PowerShell module back in the day (call it late 2011), before Microsoft had an "official" Azure cmdlets release.
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

This module provides the following cmdlets, as returned by `Get-Command -Module WAPPSCmdlets`:

| CommandType | Name                                     | ModuleName   |
| ----------- | ----                                     | ----------   |
| Cmdlet      | Add-Blob                                 | WAPPSCmdlets |
| Cmdlet      | Add-Certificate                          | WAPPSCmdlets |
| Cmdlet      | Add-DefaultPassthroughRules              | WAPPSCmdlets |
| Cmdlet      | Add-IdentityProvider                     | WAPPSCmdlets |
| Cmdlet      | Add-RelyingParty                         | WAPPSCmdlets |
| Cmdlet      | Add-Rule                                 | WAPPSCmdlets |
| Cmdlet      | Add-RuleGroup                            | WAPPSCmdlets |
| Cmdlet      | Add-ServiceIdentity                      | WAPPSCmdlets |
| Cmdlet      | Add-ServiceIdentityKey                   | WAPPSCmdlets |
| Cmdlet      | Add-TokenEncryptionKey                   | WAPPSCmdlets |
| Cmdlet      | Add-TokenSigningKey                      | WAPPSCmdlets |
| Cmdlet      | Add-TrafficManagerEndpoint               | WAPPSCmdlets |
| Cmdlet      | Clear-Container                          | WAPPSCmdlets |
| Cmdlet      | Clear-InfrastructureLog                  | WAPPSCmdlets |
| Cmdlet      | Clear-PerfmonLog                         | WAPPSCmdlets |
| Cmdlet      | Clear-WAEventLog                         | WAPPSCmdlets |
| Cmdlet      | Clear-WindowsAzureLog                    | WAPPSCmdlets |
| Cmdlet      | Get-AcsManagementToken                   | WAPPSCmdlets |
| Cmdlet      | Get-ActiveTransfers                      | WAPPSCmdlets |
| Cmdlet      | Get-AffinityGroup                        | WAPPSCmdlets |
| Cmdlet      | Get-AffinityGroups                       | WAPPSCmdlets |
| Cmdlet      | Get-Certificate                          | WAPPSCmdlets |
| Cmdlet      | Get-Certificates                         | WAPPSCmdlets |
| Cmdlet      | Get-CommonConfigurationLogs              | WAPPSCmdlets |
| Cmdlet      | Get-Container                            | WAPPSCmdlets |
| Cmdlet      | Get-Deployment                           | WAPPSCmdlets |
| Cmdlet      | Get-DiagnosticAwareRoleInstances         | WAPPSCmdlets |
| Cmdlet      | Get-DiagnosticAwareRoles                 | WAPPSCmdlets |
| Cmdlet      | Get-DiagnosticConfiguration              | WAPPSCmdlets |
| Cmdlet      | Get-HostedProperties                     | WAPPSCmdlets |
| Cmdlet      | Get-HostedService                        | WAPPSCmdlets |
| Cmdlet      | Get-HostedServices                       | WAPPSCmdlets |
| Cmdlet      | Get-IdentityProvider                     | WAPPSCmdlets |
| Cmdlet      | Get-InfrastructureLog                    | WAPPSCmdlets |
| Cmdlet      | Get-OperationStatus                      | WAPPSCmdlets |
| Cmdlet      | Get-OSVersions                           | WAPPSCmdlets |
| Cmdlet      | Get-PerfmonLog                           | WAPPSCmdlets |
| Cmdlet      | Get-RelyingParty                         | WAPPSCmdlets |
| Cmdlet      | Get-RoleInstanceCount                    | WAPPSCmdlets |
| Cmdlet      | Get-RoleInstanceStatus                   | WAPPSCmdlets |
| Cmdlet      | Get-Rule                                 | WAPPSCmdlets |
| Cmdlet      | Get-RuleGroup                            | WAPPSCmdlets |
| Cmdlet      | Get-ServiceIdentity                      | WAPPSCmdlets |
| Cmdlet      | Get-ServiceIdentityKey                   | WAPPSCmdlets |
| Cmdlet      | Get-ServiceKey                           | WAPPSCmdlets |
| Cmdlet      | Get-SqlAzureFirewallRules                | WAPPSCmdlets |
| Cmdlet      | Get-SqlAzureServer                       | WAPPSCmdlets |
| Cmdlet      | Get-StorageAccount                       | WAPPSCmdlets |
| Cmdlet      | Get-StorageAccountProperties             | WAPPSCmdlets |
| Cmdlet      | Get-StorageAnalyticsLogs                 | WAPPSCmdlets |
| Cmdlet      | Get-StorageAnalyticsMetrics              | WAPPSCmdlets |
| Cmdlet      | Get-StorageKeys                          | WAPPSCmdlets |
| Cmdlet      | Get-StorageProperties                    | WAPPSCmdlets |
| Cmdlet      | Get-StorageServicePropertiesForAnalytics | WAPPSCmdlets |
| Cmdlet      | Get-StorageServices                      | WAPPSCmdlets |
| Cmdlet      | Get-Subscription                         | WAPPSCmdlets |
| Cmdlet      | Get-TrafficManagerDefinition             | WAPPSCmdlets |
| Cmdlet      | Get-TrafficManagerProfile                | WAPPSCmdlets |
| Cmdlet      | Get-WAEventLog                           | WAPPSCmdlets |
| Cmdlet      | Get-WindowsAzureLog                      | WAPPSCmdlets |
| Cmdlet      | Import-Subscription                      | WAPPSCmdlets |
| Cmdlet      | Move-Deployment                          | WAPPSCmdlets |
| Cmdlet      | New-AffinityGroup                        | WAPPSCmdlets |
| Cmdlet      | New-Deployment                           | WAPPSCmdlets |
| Cmdlet      | New-HostedService                        | WAPPSCmdlets |
| Cmdlet      | New-PerformanceCounter                   | WAPPSCmdlets |
| Cmdlet      | New-SqlAzureFirewallRule                 | WAPPSCmdlets |
| Cmdlet      | New-SqlAzureServer                       | WAPPSCmdlets |
| Cmdlet      | New-StorageAccount                       | WAPPSCmdlets |
| Cmdlet      | New-StorageKey                           | WAPPSCmdlets |
| Cmdlet      | New-TrafficManagerDefinition             | WAPPSCmdlets |
| Cmdlet      | New-TrafficManagerEndpoint               | WAPPSCmdlets |
| Cmdlet      | New-TrafficManagerMonitor                | WAPPSCmdlets |
| Cmdlet      | New-TrafficManagerProfile                | WAPPSCmdlets |
| Cmdlet      | Remove-AffinityGroup                     | WAPPSCmdlets |
| Cmdlet      | Remove-Certificate                       | WAPPSCmdlets |
| Cmdlet      | Remove-Deployment                        | WAPPSCmdlets |
| Cmdlet      | Remove-HostedService                     | WAPPSCmdlets |
| Cmdlet      | Remove-IdentityProvider                  | WAPPSCmdlets |
| Cmdlet      | Remove-RelyingParty                      | WAPPSCmdlets |
| Cmdlet      | Remove-Rule                              | WAPPSCmdlets |
| Cmdlet      | Remove-RuleGroup                         | WAPPSCmdlets |
| Cmdlet      | Remove-ServiceIdentity                   | WAPPSCmdlets |
| Cmdlet      | Remove-ServiceIdentityKey                | WAPPSCmdlets |
| Cmdlet      | Remove-ServiceKey                        | WAPPSCmdlets |
| Cmdlet      | Remove-SqlAzureFirewallRule              | WAPPSCmdlets |
| Cmdlet      | Remove-SqlAzureServer                    | WAPPSCmdlets |
| Cmdlet      | Remove-StorageAccount                    | WAPPSCmdlets |
| Cmdlet      | Remove-Subscription                      | WAPPSCmdlets |
| Cmdlet      | Remove-TrafficManagerEndpoint            | WAPPSCmdlets |
| Cmdlet      | Remove-TrafficManagerProfile             | WAPPSCmdlets |
| Cmdlet      | Reset-RoleInstance                       | WAPPSCmdlets |
| Cmdlet      | Save-Container                           | WAPPSCmdlets |
| Cmdlet      | Select-Subscription                      | WAPPSCmdlets |
| Cmdlet      | Set-AffinityGroup                        | WAPPSCmdlets |
| Cmdlet      | Set-CommonConfigurationLogs              | WAPPSCmdlets |
| Cmdlet      | Set-Deployment                           | WAPPSCmdlets |
| Cmdlet      | Set-DeploymentConfiguration              | WAPPSCmdlets |
| Cmdlet      | Set-DeploymentStatus                     | WAPPSCmdlets |
| Cmdlet      | Set-FileBasedLog                         | WAPPSCmdlets |
| Cmdlet      | Set-HostedService                        | WAPPSCmdlets |
| Cmdlet      | Set-InfrastructureLog                    | WAPPSCmdlets |
| Cmdlet      | Set-PerformanceCounter                   | WAPPSCmdlets |
| Cmdlet      | Set-RoleInstanceCount                    | WAPPSCmdlets |
| Cmdlet      | Set-SqlAzurePassword                     | WAPPSCmdlets |
| Cmdlet      | Set-StorageAccount                       | WAPPSCmdlets |
| Cmdlet      | Set-StorageServicePropertiesForAnalytics | WAPPSCmdlets |
| Cmdlet      | Set-Subscription                         | WAPPSCmdlets |
| Cmdlet      | Set-TrafficManagerEndpoint               | WAPPSCmdlets |
| Cmdlet      | Set-TrafficManagerProfile                | WAPPSCmdlets |
| Cmdlet      | Set-WAEventLog                           | WAPPSCmdlets |
| Cmdlet      | Set-WalkUpgradeDomain                    | WAPPSCmdlets |
| Cmdlet      | Set-WindowsAzureLog                      | WAPPSCmdlets |
| Cmdlet      | Set-WindowsEventLog                      | WAPPSCmdlets |
| Cmdlet      | Start-OnDemandTransfer                   | WAPPSCmdlets |
| Cmdlet      | Stop-ActiveTransfer                      | WAPPSCmdlets |
| Cmdlet      | Update-Deployment                        | WAPPSCmdlets |
