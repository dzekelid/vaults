---
swagger: "2.0"
info:
  title: Amazon Glacier API List  Vaults
  version: 1.0.0
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
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountId}/vaults:
    get:
      summary: List  Vaults
      description: DescriptionThis operation lists all vaults owned by the calling
        user&#8217;s account
      operationId: List Vaults (GET vaults)
      parameters:
      - in: query
        name: CreationDate
        description: The date the vault was created, in Coordinated Universal Time
          (UTC)
        type: string
      - in: query
        name: LastInventoryDate
        description: The date of the last vault inventory, in Coordinated Universal
          Time (UTC)
        type: string
      - in: query
        name: Marker
        description: The vaultARN that represents where to continue pagination of
          the results
        type: string
      - in: query
        name: NumberOfArchives
        description: The number of archives in the vault as of the last inventory
          date
        type: string
      - in: query
        name: SizeInBytes
        description: "The total size, in bytes, of all the archives in the vault including
          any per-archive\t\t\t\t\t\t\t\toverhead, as of the last inventory date"
        type: string
      - in: query
        name: VaultARN
        description: The Amazon Resource Name (ARN) of the vault
        type: string
      - in: query
        name: VaultList
        description: An array of objects, with each object providing a description
          of a vault
        type: string
      - in: query
        name: VaultName
        description: The vault name
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