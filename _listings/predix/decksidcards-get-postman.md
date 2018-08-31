{
  "info": {
    "name": "Predix Views Queries cards of Deck.",
    "_postman_id": "67210c62-ef88-4cf4-bcdc-bf30b9c81475",
    "description": "Queries cards of deck..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Related",
      "item": [
        {
          "id": "9699e995-5b56-4c3e-b96b-66f90aa02aaa",
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
              "id": "4f405734-e9f9-44f4-be40-5da422186bdf"
            }
          ]
        }
      ]
    },
    {
      "name": "Queries",
      "item": [
        {
          "id": "bf797368-b5f0-46fc-8b22-4e7d416ed445",
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
              "id": "9ff5bc5a-400b-4c7b-88a0-32f365608909"
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