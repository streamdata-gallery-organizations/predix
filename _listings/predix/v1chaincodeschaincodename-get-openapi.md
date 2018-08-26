---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix BlockChain Get Chaincodes
  description: Get a single chaincode
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/chaincodes/{chaincodeName}:
    put:
      summary: Put Chaincodes
      description: Deploy chaincode (smart contract) to Blockchain
      operationId: deploy-chaincode-smart-contract-to-blockchain
      x-api-path-slug: v1chaincodeschaincodename-put
      parameters:
      - in: formData
        name: args
        description: args for uploaded script, e
      - in: header
        name: Authorization
        description: access token
      - in: formData
        name: chaincode
        description: upload compressed file (tar
      - in: path
        name: chaincodeName
        description: name of chain code
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Chaincodes
    get:
      summary: Get Chaincodes
      description: Get a single chaincode
      operationId: get-a-single-chaincode
      x-api-path-slug: v1chaincodeschaincodename-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: chaincodeName
        description: name of deployed chain code
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Chaincodes
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