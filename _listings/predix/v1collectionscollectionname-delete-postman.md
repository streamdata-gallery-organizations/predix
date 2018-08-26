{
  "info": {
    "name": "Predix Dynamic Mapping Delete a collection",
    "_postman_id": "0e941e51-3c96-4abd-b8d6-709d5b261032",
    "description": "Delete the asset collection specified by the collection name. Any associated asset and asset location data\nare also deleted",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "a3819733-1670-421e-929d-f6ead6eee681",
          "name": "returns-an-array-containing-the-names-of-all-asset-collections-for-thespecified-customer",
          "request": {
            "url": "{{default}}/v1/collections?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns an array containing the names of all asset collections for the\nspecified customer."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "c370b04b-e4df-48a8-9973-ac4e7d23e8b9"
            }
          ]
        }
      ]
    },
    {
      "name": "Return",
      "item": [
        {
          "id": "752fd8b4-d63b-4841-a65e-c9080fde6efa",
          "name": "returns-the-collection-name-and-a-list-of-ids-of-the-assets-that-belong-tothe-collection",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v1/collections/:collectionName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collectionName",
                  "value": "collectionName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the collection name and a list of ids of the assets that belong to\nthe collection."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "89c1c372-a11b-4ce0-9c1b-154398ca7122"
            }
          ]
        }
      ]
    },
    {
      "name": "Collection",
      "item": [
        {
          "id": "bd0b1c88-21cf-4d3c-a248-eef45665f019",
          "name": "delete-the-asset-collection-specified-by-the-collection-name-any-associated-asset-and-asset-location",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v1/collections/:collectionName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collectionName",
                  "value": "collectionName",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete the asset collection specified by the collection name. Any associated asset and asset location data\nare also deleted"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "30deb070-33c0-403c-a800-cd20ba39f6b0"
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