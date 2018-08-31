{
  "info": {
    "name": "Predix Insights Get Dags",
    "_postman_id": "e7fe2acc-e5ea-4640-927f-58d36e42d8c4",
    "description": "Get dags.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Dags",
      "item": [
        {
          "id": "8d4dbc43-ec15-4ca4-adb4-a05af114cb38",
          "name": "getDAGsUsingGET",
          "request": {
            "url": "http://insights-api.data-services.predix.io/api/v1/dags?maxUpdateTime=%7B%7D&minUpdateTime=%7B%7D&name=%7B%7D&page=%7B%7D&size=%7B%7D&sort=%7B%7D&tag=%7B%7D&type=%7B%7D",
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
            "description": "Get dags."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "a0321f97-f9a8-43e4-845c-281371265858"
            }
          ]
        }
      ]
    }
  ]
}