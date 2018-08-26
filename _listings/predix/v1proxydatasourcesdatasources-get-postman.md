{
  "info": {
    "name": "Predix ThetaRay Predix Service Data Sources List",
    "_postman_id": "ea0a3fe7-b8c3-40ea-b424-4697ea705d74",
    "description": "Get list of all Data Sources",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Proxy",
      "item": [
        {
          "id": "af1d9dd8-fa83-490e-bf9d-81b76db98103",
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
              "id": "620d76ba-7e63-4a3b-856f-f0805d6fc6a6"
            }
          ]
        },
        {
          "id": "a6d20121-3666-41e5-a240-b602f65d8a3a",
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
              "id": "92ff893a-a0fd-45b7-8f66-e8b96af140a1"
            }
          ]
        },
        {
          "id": "1063b4c8-9e51-401b-8edb-978696a9e661",
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
              "id": "9233cd12-f26c-4765-833e-39be6936d12b"
            }
          ]
        },
        {
          "id": "5c22bacc-25a5-4c63-a0cc-2204795aafb5",
          "name": "getDataSourcesUsingGET",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/datasources/datasources",
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
            "description": "Get list of all Data Sources"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44a8992b-b826-49ec-8a5f-d55d67424c77"
            }
          ]
        }
      ]
    }
  ]
}