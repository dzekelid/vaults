---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 0
info:
  title: CoinFabrik Delete account
  description: "Removes user\u2019s account. In order to remove an account it can\u2019t
    be\n\n- Primary account\n- Account with non-zero balance\n- Fiat account\n- Vault
    with a pending withdrawal"
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}:
    delete:
      summary: Delete account
      description: "Removes user\u2019s account. In order to remove an account it
        can\u2019t be\n\n- Primary account\n- Account with non-zero balance\n- Fiat
        account\n- Vault with a pending withdrawal"
      operationId: removes-users-account-in-order-to-remove-an-account-it-cant-be-primary-account-account-with-nonzero-
      x-api-path-slug: accountsaccount-id-delete
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Account
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