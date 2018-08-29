swagger: "2.0"
x-collection-name: PayJunction
x-complete: 1
info:
  title: PayJunction API Basic
  description: todo-add-description
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
  /customers/{customerId}/vaults/{vaultId}:
    get:
      summary: Get Customers Vaults
      description: /customers/{customerid}/vaults/{vaultid}.
      operationId: CustomersVaultsByCustomerIdAndVaultIdGet
      x-api-path-slug: customerscustomeridvaultsvaultid-get
      parameters:
      - in: path
        name: customerId
      - in: path
        name: vaultId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
    delete:
      summary: Delete Customers Vaults
      description: /customers/{customerid}/vaults/{vaultid}.
      operationId: CustomersVaultsByCustomerIdAndVaultIdDelete
      x-api-path-slug: customerscustomeridvaultsvaultid-delete
      parameters:
      - in: path
        name: customerId
      - in: path
        name: vaultId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
  /customers/{customerId}/vaults:
    post:
      summary: Post Customers Vaults
      description: /customers/{customerid}/vaults (card).
      operationId: CustomersVaultsByCustomerIdPost2
      x-api-path-slug: customerscustomeridvaults-post
      parameters:
      - in: formData
        name: address
      - in: formData
        name: addressId
      - in: formData
        name: cardExpMonth
        description: 1-12
      - in: formData
        name: cardExpYear
        description: YYYY, YY
      - in: formData
        name: cardNumber
        description: 5105105105105100,5105-1051-0510-5100,5105 1051 0510 5100
      - in: formData
        name: city
      - in: path
        name: customerId
      - in: formData
        name: state
      - in: header
        name: X-PJ-Application-Key
      - in: formData
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
  /customers/{customerId}/vaults/{achVault}:
    put:
      summary: Put Customers Vaults ACH Vault
      description: /customers/{customerid}/vaults/{vaultid} (ach).
      operationId: CustomersVaultsByCustomerIdAndAchVaultPut
      x-api-path-slug: customerscustomeridvaultsachvault-put
      parameters:
      - in: formData
        name: achAccountType
        description: CHECKING, SAVINGS
      - in: formData
        name: achType
        description: CCD, PPD, TEL, WEB
      - in: path
        name: achVault
      - in: formData
        name: address
      - in: formData
        name: addressId
      - in: formData
        name: city
      - in: path
        name: customerId
      - in: formData
        name: state
      - in: header
        name: X-PJ-Application-Key
      - in: formData
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
      - ACH
      - Vault
  /customers/{customerId}/vaults/{cardVault}:
    put:
      summary: Put Customers Vaults Card Vault
      description: /customers/{customerid}/vaults/{vaultid} (card).
      operationId: CustomersVaultsByCustomerIdAndCardVaultPut
      x-api-path-slug: customerscustomeridvaultscardvault-put
      parameters:
      - in: formData
        name: address
      - in: formData
        name: addressId
      - in: formData
        name: cardExpMonth
        description: 1-12
      - in: formData
        name: cardExpYear
        description: YYYY, YY
      - in: path
        name: cardVault
      - in: formData
        name: city
      - in: path
        name: customerId
      - in: formData
        name: state
      - in: header
        name: X-PJ-Application-Key
      - in: formData
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
      - Card
      - Vault