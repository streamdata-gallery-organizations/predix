{
  "info": {
    "name": "Predix Enterprise Connect Get EC Gateway settings",
    "_postman_id": "350a7385-6c85-4304-b3ca-f9f3906543ec",
    "description": "Get your EC Gateway settings details",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "EC",
      "item": [
        {
          "id": "80ad96a7-a572-43e3-ba58-02a732cdf73e",
          "name": "get-your-ec-gateway-settings-details",
          "request": {
            "url": "http://ec-predix-service-osaka.run.aws-usw02-pr.ice.predix.io/v1/api/settings",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer *your_token",
                "disabled": false
              },
              {
                "key": "Predix-Zone-Id",
                "value": "{}",
                "description": "",
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
            "description": "Get your EC Gateway settings details"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "3509a039-b671-4f29-a161-7e102ea33089"
            }
          ]
        }
      ]
    }
  ]
}