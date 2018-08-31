{
  "info": {
    "name": "Predix Assets Gets all user-defined domain objects.",
    "_postman_id": "0cf5d386-91af-43c8-9118-a3522fcfe1d5",
    "description": "This is a user-defined domain object collection.\n\nYou can create your own custom domain objects, add properties to them, define relationships, and so on.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Listing",
      "item": [
        {
          "id": "12af39cd-224b-43d9-984e-fa644ac95c3f",
          "name": "getV1",
          "request": {
            "url": "{{default}}/v1/",
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
            "description": "Returns the names of all user-defined domain object collections with counts of domain objects contained."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "a3f04643-90ff-45c8-8b51-638d6879245f"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "48b0de78-2bc0-4217-848a-81da48fc0a6e",
          "name": "getV1Collection",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v1/:collection"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collection",
                  "value": "{}",
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
            "description": "This is a user-defined domain object collection.\n\nYou can create your own custom domain objects, add properties to them, define relationships, and so on."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "b979b79d-3839-4ab1-855d-2e1a6bfe1277"
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