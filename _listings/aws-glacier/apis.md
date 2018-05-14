---
name: AWS Glacier
description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
  service for data archiving and long-term backup. Customers can reliably store large
  or small amounts of data for as little as $0.004 per gigabyte per month, a significant
  savings compared to on-premises solutions. To keep costs low yet suitable for varying
  retrieval needs, Amazon Glacier provides three options for access to archives, from
  a few minutes to several hours.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Storage
- Stack Network
- Amazon Web Services
created: "2018-03-24"
modified: "2018-03-24"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/aws-glacier/apis.yaml
specificationVersion: "0.14"
apis:
- name: Amazon Glacier API
  description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
    service for data archiving and long-term backup
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: ""
  baseURL: :///
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/aws-glacier/accountid-vaults-get.md
- name: Amazon Glacier API List  Vaults
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
  baseURL: http:://{host}//
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vaults/master/_listings/aws-glacier/accountid-vaults-get.md
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