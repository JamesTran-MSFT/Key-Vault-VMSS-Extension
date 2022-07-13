# Deploying a KV VMSS Extension
Reference - https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/key-vault-windows

When deploying a VMSS Extension, if you're running into the below error you can remove the `apiVersion` parameter to and redeploy the template.

{"code":"DeploymentFailed","message":"At least one resource deployment operation failed. Please list deployment operations for details. Please see https://aka.ms/DeployOperations for usage details.","details":[{"code":"BadRequest","message":"Could not find member 'apiVersion' on object of type 'VMScaleSetVMExtension'. Path 'properties.virtualMachineProfile.extensionProfile.extensions[0].apiVersion', line 1, position 1812."}]}
![image](https://user-images.githubusercontent.com/36619112/178836696-2e7d5c20-3fdd-4257-936e-d7ec0e2cf034.png)
