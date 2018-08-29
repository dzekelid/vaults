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
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/apis.md
specificationVersion: "0.14"
apis:
- name: KeyVaultManagementClient - Vaults Create Or Update
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-put
  description: Create or update a key vault in the specified subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
  humanURL: https://azure.microsoft.com/en-us/services/key-vault/
  baseURL: ://management.azure.com//
  tags: Microsoft, Authentication, Security, Management, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-put-openapi.md
- name: KeyVaultManagementClient - Vaults Delete
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-delete
  description: Deletes the specified Azure key vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
  humanURL: https://azure.microsoft.com/en-us/services/key-vault/
  baseURL: ://management.azure.com//
  tags: Microsoft, Authentication, Security, Management, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-delete-openapi.md
- name: KeyVaultManagementClient - Vaults Get
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-get
  description: Gets the specified Azure key vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
  humanURL: https://azure.microsoft.com/en-us/services/key-vault/
  baseURL: ://management.azure.com//
  tags: Microsoft, Authentication, Security, Management, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-keyvaultvaultsvaultname-get-openapi.md
- name: KeyVaultManagementClient - Vaults List
  x-api-slug: subscriptionssubscriptionidresources-get
  description: The List operation gets information about the vaults associated with
    the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-enhance-data-protection.png
  humanURL: https://azure.microsoft.com/en-us/services/key-vault/
  baseURL: ://management.azure.com//
  tags: Microsoft, Authentication, Security, Management, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/azure-key-vault/subscriptionssubscriptionidresources-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.iot.hub.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.key.vault.stack.network
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