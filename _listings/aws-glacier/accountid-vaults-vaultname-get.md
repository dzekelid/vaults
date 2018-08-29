---
swagger: "2.0"
info:
  title: Amazon Glacier API Describe  Vault
  version: 1.0.0
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
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountId}/vaults/{VaultName}:
    get:
      summary: Describe  Vault
      description: "DescriptionThis operation returns information about a vault, including
        the vault Amazon Resource Name\n\t\t\t(ARN), the date the vault was created,
        the number of archives contained within the\n\t\t\tvault, and the total size
        of all the archives in the vault"
      operationId: Describe Vault (GET vault)
      parameters:
      - in: query
        name: CreationDate
        description: The UTC date when the vault was created
        type: string
      - in: query
        name: LastInventoryDate
        description: The UTC date when Amazon Glacier completed the last vault inventory
        type: string
      - in: query
        name: NumberOfArchives
        description: The number of archives in the vault as per the last vault inventory
        type: string
      - in: query
        name: SizeInBytes
        description: "The total size in bytes of the archives in the vault including
          any per-archive overhead,\t\t\t\t\t\t\tas of the last inventory date"
        type: string
      - in: query
        name: VaultARN
        description: The Amazon Resource Name (ARN) of the vault
        type: string
      - in: query
        name: VaultName
        description: The vault name that was specified at creation time
        type: string
      responses:
        200:
          description: OK
      tags:
      - vaults
definitions: []
x-collection-name: AWS Glacier
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