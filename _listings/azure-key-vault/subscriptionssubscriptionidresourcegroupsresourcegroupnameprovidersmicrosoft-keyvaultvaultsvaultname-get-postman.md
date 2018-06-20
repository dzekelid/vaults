{
  "info": {
    "name": "Azure Key Vault API Vaults Get",
    "_postman_id": "a23026a7-6785-41f7-bcb0-41e9a489d00a",
    "description": "Gets the specified Azure key vault.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "vaults",
      "item": [
        {
          "id": "d67bf39e-fc16-4384-90b3-26d1f851a06a",
          "name": "Vaults_Get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the specified Azure key vault"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73e10b7c-5ae1-4538-ad41-105ea665fe5c"
            }
          ]
        }
      ]
    }
  ]
}