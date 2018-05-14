{
  "info": {
    "name": "Azure Key Vault API Vaults List By Resource Group",
    "_postman_id": "fd85d4b5-974a-4190-8860-c2f4678e5912",
    "description": "The List operation gets information about the vaults associated with the subscription and within the specified resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "vaults resource group",
      "item": [
        {
          "id": "c423e428-4594-4832-9564-46f6ed00c707",
          "name": "Vaults_ListByResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.KeyVault/vaults"
              ],
              "query": [
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The List operation gets information about the vaults associated with the subscription and within the specified resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76b83c13-b7dc-43a2-94e6-b8949abfcd89"
            }
          ]
        }
      ]
    }
  ]
}