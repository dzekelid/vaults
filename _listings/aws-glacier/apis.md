---
name: AWS Glacier
x-slug: aws-glacier
description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
  service for data archiving and long-term backup. Customers can reliably store large
  or small amounts of data for as little as $0.004 per gigabyte per month, a significant
  savings compared to on-premises solutions. To keep costs low yet suitable for varying
  retrieval needs, Amazon Glacier provides three options for access to archives, from
  a few minutes to several hours.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Vaults
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/aws-glacier/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Glacier API Create  Vault
  x-api-slug: amazon-glacier-api
  description: "DescriptionThis operation creates a new vault with the specified name.&nbsp;
    The name of the vault must be\n\t\t\tunique within a region for an AWS account.
    You can create up to 1,000 vaults per\n\t\t\taccount. For information on creating
    more vaults, go to the Amazon Glacier product detail\n\t\t\tpage.You must use
    the following guidelines when naming a vault. \n\t\t\t Names can be between 1
    and 255 characters long. Allowed characters are a&#8211;z, A&#8211;Z, 0&#8211;9,
    '_' (underscore), '-' (hyphen),\n\t\t\t\t\t\tand '.' (period).\n\t\tThis operation
    is idempotent, you can send the same request multiple times and it has no\n\t\t\tfurther
    effect after the first time Amazon Glacier creates the specified vault.Requests"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/aws-glacier/accountidvaultsvaultname-put-openapi.md
- name: Amazon Glacier API Delete  Vault
  x-api-slug: amazon-glacier-api
  description: "DescriptionThis operation deletes a vault. Amazon Glacier will delete
    a vault only if there are no archives\n\t\t\tin the vault as per the last inventory
    and there have been no writes to the vault since\n\t\t\tthe last inventory. If
    either of these conditions is not satisfied, the vault deletion\n\t\t\tfails (that
    is, the vault is not removed) and Amazon Glacier returns an error. You can use
    the Describe Vault (GET vault)\n\t\t\toperation that provides vault information,
    including the number of archives in the vault;\n\t\t\thowever, the information
    is based on the vault inventory Amazon Glacier last\n\t\t\tgenerated.This operation
    is idempotent.NoteWhen you delete a vault, the vault access policy attached to
    the vault is also deleted. \n\t\t\t\tFor more information about vault access policies,
    see Amazon Glacier Access Control with Vault Access Policies.RequestsTo delete
    a vault, send a DELETE request to the vault resource URI."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/aws-glacier/accountidvaultsvaultname-delete-openapi.md
- name: Amazon Glacier API Describe  Vault
  x-api-slug: amazon-glacier-api
  description: "DescriptionThis operation returns information about a vault, including
    the vault Amazon Resource Name\n\t\t\t(ARN), the date the vault was created, the
    number of archives contained within the\n\t\t\tvault, and the total size of all
    the archives in the vault. The number of archives and\n\t\t\ttheir total size
    are as of the last vault inventory Amazon Glacier generated (see Working with
    Vaults in Amazon Glacier). Amazon Glacier\n\t\t\tgenerates vault inventories approximately
    daily. This means that if you add or remove an\n\t\t\tarchive from a vault, and
    then immediately send a Describe Vault request, the response\n\t\t\tmight not
    reflect the changes.  RequestsTo get information about a vault, send a GET request
    to the URI of the specific\n\t\t\tvault resource."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/aws-glacier/accountidvaultsvaultname-get-openapi.md
- name: Amazon Glacier API List  Vaults
  x-api-slug: amazon-glacier-api
  description: "DescriptionThis operation lists all vaults owned by the calling user&#8217;s
    account. The list returned in\n\t\t\tthe response is ASCII-sorted by vault name.
    By default, this operation returns up to 1,000 items per request. If there are
    more vaults\n\t\t\tto list, the marker field in the response body contains the
    vault Amazon\n\t\t\tResource Name (ARN) at which to continue the list with a new
    List Vaults request;\n\t\t\totherwise, the marker field is null. In your next
    List Vaults\n\t\t\trequest you set the marker parameter to the value Amazon Glacier
    returned in the\n\t\t\tresponses to your previous List Vaults request. You can
    also limit the number of vaults\n\t\t\treturned in the response by specifying
    the limit parameter in the request. RequestsTo get a list of vaults, you send
    a GET request to the\n\t\t\t\tvaults resource."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/aws-glacier/accountidvaults-get-openapi.md
- name: Amazon Glacier API
  x-api-slug: amazon-glacier-api
  description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
    service for data archiving and long-term backup. Customers can reliably store
    large or small amounts of data for as little as $0.004 per gigabyte per month,
    a significant savings compared to on-premises solutions. To keep costs low yet
    suitable for varying retrieval needs, Amazon Glacier provides three options for
    access to archives, from a few minutes to several hours.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: :///
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/aws-glacier/openapi.md
x-common:
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/Amazon-Glacier/
- type: x-documentation
  url: http://docs.aws.amazon.com/amazonglacier/latest/dev/amazon-glacier-api.html
- type: x-faq
  url: https://aws.amazon.com/glacier/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=140
- type: x-getting-started
  url: https://aws.amazon.com/glacier/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/glacier/pricing/
- type: x-website
  url: https://aws.amazon.com/glacier/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---