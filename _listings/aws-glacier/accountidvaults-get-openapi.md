---
swagger: "2.0"
x-collection-name: AWS Glacier
x-complete: 0
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
  /{AccountId}/vaults/{VaultName}:
    put:
      summary: Create  Vault
      description: "DescriptionThis operation creates a new vault with the specified
        name.&nbsp; The name of the vault must be\n\t\t\tunique within a region for
        an AWS account. You can create up to 1,000 vaults per\n\t\t\taccount. For
        information on creating more vaults, go to the Amazon Glacier product detail\n\t\t\tpage.You
        must use the following guidelines when naming a vault. \n\t\t\t Names can
        be between 1 and 255 characters long. Allowed characters are a&#8211;z, A&#8211;Z,
        0&#8211;9, '_' (underscore), '-' (hyphen),\n\t\t\t\t\t\tand '.' (period).\n\t\tThis
        operation is idempotent, you can send the same request multiple times and
        it has no\n\t\t\tfurther effect after the first time Amazon Glacier creates
        the specified vault.Requests"
      operationId: Create Vault (PUT vault)
      x-api-path-slug: accountidvaultsvaultname-put
      parameters:
      - type: string
      responses:
        200:
          description: OK
      tags:
      - Vaults
    delete:
      summary: Delete  Vault
      description: "DescriptionThis operation deletes a vault. Amazon Glacier will
        delete a vault only if there are no archives\n\t\t\tin the vault as per the
        last inventory and there have been no writes to the vault since\n\t\t\tthe
        last inventory. If either of these conditions is not satisfied, the vault
        deletion\n\t\t\tfails (that is, the vault is not removed) and Amazon Glacier
        returns an error. You can use the Describe Vault (GET vault)\n\t\t\toperation
        that provides vault information, including the number of archives in the vault;\n\t\t\thowever,
        the information is based on the vault inventory Amazon Glacier last\n\t\t\tgenerated.This
        operation is idempotent.NoteWhen you delete a vault, the vault access policy
        attached to the vault is also deleted. \n\t\t\t\tFor more information about
        vault access policies, see Amazon Glacier Access Control with Vault Access
        Policies.RequestsTo delete a vault, send a DELETE request to the vault resource
        URI."
      operationId: Delete Vault (DELETE vault)
      x-api-path-slug: accountidvaultsvaultname-delete
      responses:
        200:
          description: OK
      tags:
      - Vaults
    get:
      summary: Describe  Vault
      description: "DescriptionThis operation returns information about a vault, including
        the vault Amazon Resource Name\n\t\t\t(ARN), the date the vault was created,
        the number of archives contained within the\n\t\t\tvault, and the total size
        of all the archives in the vault. The number of archives and\n\t\t\ttheir
        total size are as of the last vault inventory Amazon Glacier generated (see
        Working with Vaults in Amazon Glacier). Amazon Glacier\n\t\t\tgenerates vault
        inventories approximately daily. This means that if you add or remove an\n\t\t\tarchive
        from a vault, and then immediately send a Describe Vault request, the response\n\t\t\tmight
        not reflect the changes.  RequestsTo get information about a vault, send a
        GET request to the URI of the specific\n\t\t\tvault resource."
      operationId: Describe Vault (GET vault)
      x-api-path-slug: accountidvaultsvaultname-get
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
        description: The total size in bytes of the archives in the vault including
          any per-archive overhead,as of the last inventory date
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
      - Vaults
  /{AccountId}/vaults:
    get:
      summary: List  Vaults
      description: "DescriptionThis operation lists all vaults owned by the calling
        user&#8217;s account. The list returned in\n\t\t\tthe response is ASCII-sorted
        by vault name. By default, this operation returns up to 1,000 items per request.
        If there are more vaults\n\t\t\tto list, the marker field in the response
        body contains the vault Amazon\n\t\t\tResource Name (ARN) at which to continue
        the list with a new List Vaults request;\n\t\t\totherwise, the marker field
        is null. In your next List Vaults\n\t\t\trequest you set the marker parameter
        to the value Amazon Glacier returned in the\n\t\t\tresponses to your previous
        List Vaults request. You can also limit the number of vaults\n\t\t\treturned
        in the response by specifying the limit parameter in the request. RequestsTo
        get a list of vaults, you send a GET request to the\n\t\t\t\tvaults resource."
      operationId: List Vaults (GET vaults)
      x-api-path-slug: accountidvaults-get
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
        description: The total size, in bytes, of all the archives in the vault including
          any per-archiveoverhead, as of the last inventory date
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