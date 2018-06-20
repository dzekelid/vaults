{
  "info": {
    "name": "Azure Recovery Service API Vaults Delete",
    "_postman_id": "c66e185f-fe80-4bce-892e-000030167327",
    "description": "Deletes a vault.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "vaults",
      "item": [
        {
          "id": "91958bfa-14e1-4f60-bb03-51a255a8087d",
          "name": "Vaults_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a vault"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9164b7fa-98de-4413-bebd-9864752a31b7"
            }
          ]
        }
      ]
    }
  ]
}