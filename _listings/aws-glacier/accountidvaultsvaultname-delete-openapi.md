---
swagger: "2.0"
x-collection-name: AWS Glacier
x-complete: 0
info:
  title: Amazon Glacier API Delete  Vault
  version: 1.0.0
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