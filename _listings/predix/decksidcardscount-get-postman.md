{
  "info": {
    "name": "Predix Views Counts cards of Deck.",
    "_postman_id": "9650730d-e30d-423d-8be9-1a42fe1a8691",
    "description": "Counts cards of deck..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Related",
      "item": [
        {
          "id": "e02e7b0c-9070-4c18-b22a-0fe8dc2aee69",
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
              "id": "4d5629f2-006e-454c-b6bd-ff1fdf6d2b76"
            }
          ]
        }
      ]
    },
    {
      "name": "Queries",
      "item": [
        {
          "id": "17068f1c-a596-4a4d-ba06-fdfd1179d58c",
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
              "id": "7c8e1282-94b4-473f-9adf-e35b1409b516"
            }
          ]
        }
      ]
    },
    {
      "name": "Counts",
      "item": [
        {
          "id": "adfb4a36-ed27-4b2a-802c-29c58e0a7739",
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
              "id": "01c6206c-b313-4852-b922-dadf99802f36"
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