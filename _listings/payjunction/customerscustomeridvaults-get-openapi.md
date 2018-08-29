---
swagger: "2.0"
x-collection-name: PayJunction
x-complete: 0
info:
  title: PayJunction Get Customers Vaults
  description: Retrieve customer's payment vaults
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers/{customerId}/vaults/:
    get:
      summary: Get Customers Vaults
      description: Retrieve customer's payment vaults
      operationId: CustomersVaultsByCustomerIdGet
      x-api-path-slug: customerscustomeridvaults-get
      parameters:
      - in: path
        name: customerId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
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