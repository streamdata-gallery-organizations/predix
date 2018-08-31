{
  "info": {
    "name": "Predix BlockChain Get Chaincodes",
    "_postman_id": "8ab84547-dd9c-4dc8-8ac2-278e654eff09",
    "description": "Get all chaincodes",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Chaincodes",
      "item": [
        {
          "id": "ce04163f-aea4-4750-a7a6-1ec993c05a85",
          "name": "get-a-single-chaincode",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v1/chaincodes/:chaincodeName"
              ],
              "variable": [
                {
                  "id": "chaincodeName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "access token",
                "disabled": false
              },
              {
                "key": "predix-zone-id",
                "value": "{}",
                "description": "tenantId",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a single chaincode"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e2e9eda-f23f-4a2f-860d-9eff8b0f9a38"
            }
          ]
        },
        {
          "id": "b2361925-7a8e-4b5d-a063-bf496bc3f9fc",
          "name": "deploy-chaincode-smart-contract-to-blockchain",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v1/chaincodes/:chaincodeName"
              ],
              "variable": [
                {
                  "id": "chaincodeName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "access token",
                "disabled": false
              },
              {
                "key": "predix-zone-id",
                "value": "{}",
                "description": "tenantId",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "args",
                  "value": "{}",
                  "disabled": false,
                  "description": "args for uploaded script, e"
                },
                {
                  "key": "chaincode",
                  "value": "{}",
                  "disabled": false,
                  "description": "upload compressed file (tar"
                }
              ]
            },
            "description": "Deploy chaincode (smart contract) to Blockchain"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66723184-1372-4394-9d86-f1a1d226e16a"
            }
          ]
        },
        {
          "id": "d3c9fb46-fba0-446a-af60-392760bf18d2",
          "name": "get-all-chaincodes",
          "request": {
            "url": "{{default}}/v1/chaincodes",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "access token",
                "disabled": false
              },
              {
                "key": "predix-zone-id",
                "value": "{}",
                "description": "tenantId",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all chaincodes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb482304-f026-4ab6-98cf-8d1967bc2b9c"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/"
    }
  ]
}