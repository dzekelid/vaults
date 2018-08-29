{
  "info": {
    "name": "Azure Recovery Service API Vaults List By Subscription Id",
    "_postman_id": "cd121f9a-2c8d-47cb-af9f-34b0435edb3d",
    "description": "Fetches all the resources of the specified type in the subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "vaults subscription",
      "item": [
        {
          "id": "68d24b13-5476-4a7b-b5da-69701ad3898f",
          "name": "Vaults_ListBySubscriptionId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.RecoveryServices/vaults"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches all the resources of the specified type in the subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f39c288-ab0c-4172-8d54-8e8e9982165a"
            }
          ]
        }
      ]
    }
  ]
}