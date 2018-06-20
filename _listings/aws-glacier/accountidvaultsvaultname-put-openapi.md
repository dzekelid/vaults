---
swagger: "2.0"
x-collection-name: AWS Glacier
x-complete: 0
info:
  title: Amazon Glacier API Create  Vault
  version: 1.0.0
  description: "DescriptionThis operation creates a new vault with the specified name.&nbsp;
    The name of the vault must be\n\t\t\tunique within a region for an AWS account.
    You can create up to 1,000 vaults per\n\t\t\taccount. For information on creating
    more vaults, go to the Amazon Glacier product detail\n\t\t\tpage.You must use
    the following guidelines when naming a vault. \n\t\t\t Names can be between 1
    and 255 characters long. Allowed characters are a&#8211;z, A&#8211;Z, 0&#8211;9,
    '_' (underscore), '-' (hyphen),\n\t\t\t\t\t\tand '.' (period).\n\t\tThis operation
    is idempotent, you can send the same request multiple times and it has no\n\t\t\tfurther
    effect after the first time Amazon Glacier creates the specified vault.Requests"
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