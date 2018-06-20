---
name: Azure Key Vault
x-slug: azure-key-vault
description: Azure Key Vault offers an easy, cost-effective way to safeguard keys
  and other secrets in the cloud by using hardware security modules (HSMs). Protect
  cryptographic keys and small secrets like passwords with keys stored in HSMs. For
  added assurance, import or generate your keys in HSMs that are certified to FIPS
  140-2 level 2 and Common Criteria EAL4+ standards, so that your keys stay within
  the HSM boundary. Key Vault is designed so that Microsoft does not see or extract
  your keys. Create new keys for Dev-Test in minutes and migrate seamlessly to production
  keys managed by security operations. Key Vault scales to meet the demands of your
  cloud applications without the hassle required to provision, deploy, and manage
  HSMs and key management software.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Vaults
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Key Vault API Vaults Create Or Update
  x-api-slug: azure-key-vault-api
  description: Create or update a key vault in the specified subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
  humanURL: https://azure.microsoft.com/en-us/services/key-vault/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.KeyVault/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-put-openapi.md
- name: Azure Key Vault API Vaults Delete
  x-api-slug: azure-key-vault-api
  description: Deletes the specified Azure key vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
  humanURL: https://azure.microsoft.com/en-us/services/key-vault/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.KeyVault/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-delete-openapi.md
- name: Azure Key Vault API Vaults Get
  x-api-slug: azure-key-vault-api
  description: Gets the specified Azure key vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
  humanURL: https://azure.microsoft.com/en-us/services/key-vault/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.KeyVault/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-get-openapi.md
- name: Azure Key Vault API Vaults List By Resource Group
  x-api-slug: azure-key-vault-api
  description: The List operation gets information about the vaults associated with
    the subscription and within the specified resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
  humanURL: https://azure.microsoft.com/en-us/services/key-vault/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.KeyVault/vaults
  tags: Vaults Resource Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaults-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaults-get-openapi.md
- name: Azure Key Vault API Vaults List
  x-api-slug: azure-key-vault-api
  description: The List operation gets information about the vaults associated with
    the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
  humanURL: https://azure.microsoft.com/en-us/services/key-vault/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resources
  tags: Vaults
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresources-get-openapi.md
- name: Azure Key Vault API
  x-api-slug: azure-key-vault-api
  description: Azure Key Vault offers an easy, cost-effective way to safeguard keys
    and other secrets in the cloud by using hardware security modules (HSMs). Protect
    cryptographic keys and small secrets like passwords with keys stored in HSMs.
    For added assurance, import or generate your keys in HSMs that are certified to
    FIPS 140-2 level 2 and Common Criteria EAL4+ standards, so that your keys stay
    within the HSM boundary. Key Vault is designed so that Microsoft does not see
    or extract your keys. Create new keys for Dev-Test in minutes and migrate seamlessly
    to production keys managed by security operations. Key Vault scales to meet the
    demands of your cloud applications without the hassle required to provision, deploy,
    and manage HSMs and key management software.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
  humanURL: https://azure.microsoft.com/en-us/services/key-vault/
  baseURL: ://management.azure.com//
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/key-vault/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/key-vault/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/key-vault/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/key-vault/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---