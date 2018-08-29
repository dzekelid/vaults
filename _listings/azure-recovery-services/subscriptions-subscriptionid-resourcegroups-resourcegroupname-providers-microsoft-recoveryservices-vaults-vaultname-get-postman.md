{
  "info": {
    "name": "Azure Recovery Service API Vaults Get",
    "_postman_id": "a43cc0be-d51a-4731-9f38-b431dbabbb7a",
    "description": "Get the Vault details.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "vaults",
      "item": [
        {
          "id": "1fd41cc9-9c13-480d-bcab-d01a9605cc8e",
          "name": "Vaults_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.RecoveryServices/vaults/:vaultName"
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
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "vaultName",
                  "value": "vaultName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the Vault details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a1473d1-6fcc-40d6-9ef7-15ed4ecfc1a0"
            }
          ]
        }
      ]
    }
  ]
}