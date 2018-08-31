{
  "info": {
    "name": "Predix AppHub ARCS Get all the registered microapps",
    "_postman_id": "81f162c4-21aa-44e7-82c2-c8318107490d",
    "description": "Get the registered microapps for the given tenant",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Apps",
      "item": [
        {
          "id": "35f2debd-e106-4a81-b9fd-40f91d7f96d9",
          "name": "getAllRegisteredAppsUsingGET",
          "request": {
            "url": "http://predix-apphub-arcs-prod.run.aws-usw02-pr.ice.predix.io/api/apps",
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
            "description": "Get the registered microapps for the given tenant"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84e77f7b-abdb-46e9-a5d2-810fdcd80eb8"
            }
          ]
        }
      ]
    }
  ]
}