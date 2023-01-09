# AMA
## to trigger policy
az policy state trigger-scan

### to list extntion 
Get-AzVMImagePublisher -location usgovvirginia | Get-AzVMExtensionImagetype | ?{$_.PublisherName -like "Microsoft.Azure.Monitor"} | Get-AzVMExtensionImage![image](https://user-images.githubusercontent.com/52181728/211374405-8166e228-f61e-433b-9acc-f6380f805718.png)
