#  ImageUpload Webapp

ARM template that create Azure Web application for uploading images to Storage Account using SAS key.

## Notes

Webapp is created by [Gaurav Mantri](https://gauravmantri.com/2013/02/16/uploading-large-files-in-windows-azure-blob-storage-using-shared-access-signature-html-and-javascript/)

## Deploying from PowerShell

- Open PowerShell and Login into Azure
- Create Resource Group
- Run New-AzureRmResourceGroupDeployment command

```
New-AzureRmResourceGroup -Name imageupload003 -Location "west europe"
```
```
New-AzureRmResourceGroupDeployment -Name imageupload003 -ResourceGroupName imageupload003 -TemplateUri https://raw.githubusercontent.com/JurislavP/Azure_
MAS/master/templates/image_upload/webapp_imageupload.json -TemplateParameterUri https://raw.githubusercontent.com/JurislavP/Azure_MAS/master/templates/image_upload/webapp_imageupload_parameter.json
```