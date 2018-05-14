{
  "info": {
    "name": "Azure Key Vault API Vaults Delete",
    "_postman_id": "633a9e1f-b84f-4e84-8b1d-0488e367efe3",
    "description": "Deletes the specified Azure key vault.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "vaults",
      "item": [
        {
          "id": "6f20547e-6d4e-4d0b-83cd-5d36f1c61eb2",
          "name": "Vaults_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.KeyVault/vaults/:vaultName"
              ],
              "query": [
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
                  "id": "vaultName",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Azure key vault"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "971bfae7-34d5-4043-bc3b-7d6281ab2b43"
            }
          ]
        }
      ]
    }
  ]
}