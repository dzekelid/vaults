---
name: Azure Recovery Services
x-slug: azure-recovery-services
description: Learn how to use Site Recovery for business continuity and disaster recovery
  strategy for private clouds. Tutorials and other documentation show you how to plan,
  deploy, and manage the orchestration of replicating on-premises physical servers
  and virtual machines to the cloud or to a secondary datacenter.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Vaults
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Recovery Service API Vaults List By Subscription Id
  x-api-slug: azure-recovery-service-api
  description: Fetches all the resources of the specified type in the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/vaults
  tags: Vaults Subscription
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidprovidersmicrosoft-recoveryservicesvaults-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidprovidersmicrosoft-recoveryservicesvaults-get-openapi.md
- name: Azure Recovery Service API Vaults List By Resource Group
  x-api-slug: azure-recovery-service-api
  description: Retrieve a list of Vaults.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults
  tags: Vaults Resource Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaults-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaults-get-openapi.md
- name: Azure Recovery Service API Vaults Get
  x-api-slug: azure-recovery-service-api
  description: Get the Vault details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultname-get-openapi.md
- name: Azure Recovery Service API Vaults Create Or Update
  x-api-slug: azure-recovery-service-api
  description: Creates or updates a Recovery Services vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultname-put-openapi.md
- name: Azure Recovery Service API Vaults Delete
  x-api-slug: azure-recovery-service-api
  description: Deletes a vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultname-delete-openapi.md
- name: Azure Recovery Service API Vaults Update
  x-api-slug: azure-recovery-service-api
  description: Updates the vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultname-patch-openapi.md
- name: Azure Recovery Service API Usages List By Vaults
  x-api-slug: azure-recovery-service-api
  description: Fetches the usages of the vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/usages
  tags: Usages Vaults
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnameusages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnameusages-get-openapi.md
- name: Azure Recovery Service API
  x-api-slug: azure-recovery-service-api
  description: Learn how to use Site Recovery for business continuity and disaster
    recovery strategy for private clouds. Tutorials and other documentation show you
    how to plan, deploy, and manage the orchestration of replicating on-premises physical
    servers and virtual machines to the cloud or to a secondary datacenter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com//
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-recovery-services/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/site-recovery/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/site-recovery/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/site-recovery/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/site-recovery/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---