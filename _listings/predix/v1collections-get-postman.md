{
  "info": {
    "name": "Predix Intelligent Mapping List all data collections for a customer",
    "_postman_id": "70aa2d95-e9d5-4912-b8f1-2292a96e03a8",
    "description": "Returns an array containing the names of all data collections for the\nspecified customer.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "5c28ead9-81dc-41d8-819d-8a5b27395b54",
          "name": "returns-an-array-containing-the-names-of-all-data-collections-for-thespecified-customer",
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
            "description": "Returns an array containing the names of all data collections for the\nspecified customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f544f10-96be-4235-983e-476291b29acb"
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