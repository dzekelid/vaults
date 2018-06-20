---
swagger: "2.0"
x-collection-name: Azure Recovery Services
x-complete: 0
info:
  title: Azure Recovery Service API Vaults Get
  version: 1.0.0
  description: Get the Vault details.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/vaults:
    get:
      summary: Vaults List By Subscription Id
      description: Fetches all the resources of the specified type in the subscription.
      operationId: Vaults_ListBySubscriptionId
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-recoveryservicesvaults-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vaults Subscription
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults:
    get:
      summary: Vaults List By Resource Group
      description: Retrieve a list of Vaults.
      operationId: Vaults_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaults-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vaults Resource Group
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}:
    get:
      summary: Vaults Get
      description: Get the Vault details.
      operationId: Vaults_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultname-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vaults
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---