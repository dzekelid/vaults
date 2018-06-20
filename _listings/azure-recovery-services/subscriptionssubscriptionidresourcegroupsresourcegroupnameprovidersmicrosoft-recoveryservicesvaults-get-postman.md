{
  "info": {
    "name": "Azure Recovery Service API Vaults List By Resource Group",
    "_postman_id": "eb26ae65-740f-48a1-82d0-a3657881039b",
    "description": "Retrieve a list of Vaults.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "vaults resource group",
      "item": [
        {
          "id": "a79405a5-dd09-4bb1-aa58-8d01cfaf86d7",
          "name": "Vaults_ListByResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.RecoveryServices/vaults"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a list of Vaults"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c09d822c-c830-492b-87d7-545a0e9e3093"
            }
          ]
        }
      ]
    }
  ]
}