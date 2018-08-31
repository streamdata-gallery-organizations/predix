{
  "info": {
    "name": "Predix BlockChain Get Chaincodes",
    "_postman_id": "4391d027-7352-4a02-b1f3-339132f247ef",
    "description": "Get a single chaincode",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Chaincodes",
      "item": [
        {
          "id": "bcf2ea67-a43b-4eac-b50d-61559da959c9",
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
              "id": "59b2454c-ab9f-4419-9e1b-152b0d4be8eb"
            }
          ]
        },
        {
          "id": "2ccfca81-5243-455b-8e1a-1bf7c044d359",
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
              "id": "f823bc8b-0142-4c44-bb88-40879f06c7a4"
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