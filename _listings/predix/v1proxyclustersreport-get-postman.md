{
  "info": {
    "name": "Predix ThetaRay Predix Service Clusters Report",
    "_postman_id": "100505bd-cedc-4a47-b387-191a1d09d19e",
    "description": "Get Clusters report",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Proxy",
      "item": [
        {
          "id": "38dc5d92-64ee-45e2-b386-0c2a362fe76b",
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
              "id": "41c328f0-6fb4-40ad-b7b3-0a9980f0777a"
            }
          ]
        },
        {
          "id": "f2e0c9a6-51d6-4f1d-9949-15a821c85e32",
          "name": "retrieveReportUsingGET",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/anomalies/report?analysisId=%7B%7D&dataSourceName=%7B%7D&fromAnomaly=%7B%7D&numOfTopFeatures=%7B%7D&toAnomaly=%7B%7D",
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
            "description": "Retrieves Anomalies Report"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e04a8f8-36ca-4a18-b944-bfaf226cfea8"
            }
          ]
        },
        {
          "id": "dc384baa-d66c-4146-b3da-3a16bc833d94",
          "name": "getClustersReportUsingGET",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/clusters/report?analysisId=%7B%7D&dataSourceName=%7B%7D&filterOnlyUsedToCluster=%7B%7D&fromAnomaly=%7B%7D&toAnomaly=%7B%7D&withMinClusterSize=%7B%7D",
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
            "description": "Get Clusters report"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa637806-1a72-4af4-8f85-36a00b0be4ce"
            }
          ]
        }
      ]
    }
  ]
}