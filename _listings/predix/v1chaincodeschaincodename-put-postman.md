{
  "info": {
    "name": "Predix BlockChain Put Chaincodes",
    "_postman_id": "c89c91e0-9861-466d-96d8-bab9e2dfbb84",
    "description": "Deploy chaincode (smart contract) to Blockchain",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Chaincodes",
      "item": [
        {
          "id": "cfbd13e8-9a56-4bf3-9fe7-debde9cea653",
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
              "id": "e1d78faf-6503-493e-aa33-f763df696578"
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