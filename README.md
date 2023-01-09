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
