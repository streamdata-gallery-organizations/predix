{
  "info": {
    "name": "Predix Assets Get a listing of user-defined domain object collections",
    "_postman_id": "0cfaf2c9-9d9e-4cf5-bb4a-7b8d81fcd747",
    "description": "Returns the names of all user-defined domain object collections with counts of domain objects contained.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Listing",
      "item": [
        {
          "id": "40dd0c4e-d65d-43c3-b51a-3cbe3c6be091",
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
              "id": "72516102-c313-4322-a397-c2d7a29bbf4f"
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