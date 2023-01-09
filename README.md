# AMA

## to trigger policy
```bash
az policy state trigger-scan
```
### to list extntion 
```bash
Get-AzVMImagePublisher -location usgovvirginia | Get-AzVMExtensionImagetype | ?{$_.PublisherName -like "Microsoft.Azure.Monitor"} | Get-AzVMExtensionImage
```

### to validate from LAW
```bash
Heartbeat | where Category == "Azure Monitor Agent" and Computer == "onprem-srv1" | take 10
```
### t-shooting doc
(https://learn.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-troubleshoot-windows-arc#basic-troubleshooting-steps-installation-agent-not-running-configuration-issues)


### from arc VM run
```bash
azcmagent show
```
