---
swagger: "2.0"
x-collection-name: Azure Recovery Services
x-complete: 1
info:
  title: RecoveryServicesClient
  version: 1.0.0
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
    put:
      summary: Vaults Create Or Update
      description: Creates or updates a Recovery Services vault.
      operationId: Vaults_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultname-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: vault
        description: Recovery Services Vault to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Vaults
    delete:
      summary: Vaults Delete
      description: Deletes a vault.
      operationId: Vaults_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultname-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vaults
    patch:
      summary: Vaults Update
      description: Updates the vault.
      operationId: Vaults_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultname-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: vault
        description: Recovery Services Vault to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Vaults
  ? /Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/usages
  : get:
      summary: Usages List By Vaults
      description: Fetches the usages of the vault.
      operationId: Usages_ListByVaults
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnameusages-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Usages Vaults
---