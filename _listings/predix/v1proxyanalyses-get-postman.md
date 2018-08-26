{
  "info": {
    "name": "Predix ThetaRay Predix Service Analyses List",
    "_postman_id": "5440df47-5684-471e-9caa-68460f7ce66b",
    "description": "Get list of Analyses",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Proxy",
      "item": [
        {
          "id": "33e58fcc-9c01-4258-9b56-78468a43d51e",
          "name": "retrieveNewUsingGET",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/analyses",
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
            "description": "Get list of Analyses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6aae57f4-25fa-48c7-8975-079468ec099e"
            }
          ]
        }
      ]
    }
  ]
}