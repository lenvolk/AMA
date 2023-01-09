# AMA

## to trigger policy
```bash
az policy state trigger-scan
```
### to list extntion 
```bash
Get-AzVMImagePublisher -location usgovvirginia | Get-AzVMExtensionImagetype | ?{$_.PublisherName -like "Microsoft.Azure.Monitor"} | Get-AzVMExtensionImage
```
