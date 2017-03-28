# Accessing Azure KeyVault from Azure Functions

This sample is for Azure Functions based on the article [Use Azure Key Vault from a Web Application](https://docs.microsoft.com/en-us/azure/key-vault/key-vault-use-from-web-application).

To run this project locally, use the Auzre CLI.

    func settings add ClientId "[AAD app client id]"
    func settings add ClientSecret "[AAD app client secret]"
    func settings add SecretUri "https://[keyvalutname].vault.azure.net/secrets/[secret name]/[secret version]"

To run the project in Azure Functions:
1. upload the `run.csx` and `project.json` files to your Azure Function
2. add app settings for ClientId, ClientSecret and SecretUri