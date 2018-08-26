{
  "info": {
    "name": "Predix Views Queries tags of Deck.",
    "_postman_id": "fdc790c3-070d-4f8b-be07-c2f78b495d6d",
    "description": "Queries tags of deck..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Related",
      "item": [
        {
          "id": "ac2af664-e668-456e-ad38-a403e2f49323",
          "name": "deleteDecksTagsFk",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "decks/:id/tags/:fk"
              ],
              "variable": [
                {
                  "id": "fk",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
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
            "description": "Delete a related item by id for tags.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e651f3b-ca4d-4957-965a-f9971b80aa06"
            }
          ]
        }
      ]
    },
    {
      "name": "Queries",
      "item": [
        {
          "id": "e08cdc4f-45d0-4a09-8adf-fa665ebadc09",
          "name": "getDecksCards",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "decks/:id/cards"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Queries cards of deck.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1dfb97b4-7f98-44df-ba71-fc79ceac1f49"
            }
          ]
        },
        {
          "id": "c4bb99ac-63c3-41f2-9069-c64b8572c521",
          "name": "getDecksTags",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "decks/:id/tags"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Queries tags of deck.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41c2b051-3c88-4ddd-929d-4a7b185f3433"
            }
          ]
        }
      ]
    },
    {
      "name": "Counts",
      "item": [
        {
          "id": "321abac8-7f3d-4bf3-83b8-a37fdeda047d",
          "name": "getDecksCardsCount",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "decks/:id/cards/count"
              ],
              "query": [
                {
                  "key": "where",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Counts cards of deck.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "165a712e-0f0e-4935-b3cc-8d529acece6c"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/v1"
    }
  ]
}