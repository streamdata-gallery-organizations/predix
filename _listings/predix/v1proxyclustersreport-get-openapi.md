---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix ThetaRay Predix Service Clusters Report
  description: Get Clusters report
  contact:
    name: supportforpredix@thetaray.com
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/proxy/analyses:
    get:
      summary: Analyses List
      description: Get list of Analyses
      operationId: retrieveNewUsingGET
      x-api-path-slug: v1proxyanalyses-get
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Analyses
  /v1/proxy/anomalies/report:
    get:
      summary: Anomalies Report
      description: Retrieves Anomalies Report
      operationId: retrieveReportUsingGET
      x-api-path-slug: v1proxyanomaliesreport-get
      parameters:
      - in: query
        name: analysisId
        description: Analysis Id
      - in: query
        name: dataSourceName
        description: Data Source name
      - in: query
        name: fromAnomaly
        description: Fetch from Anomaly in Analysis
      - in: query
        name: numOfTopFeatures
        description: Number of top features to fetch
      - in: query
        name: toAnomaly
        description: Fetch up to Anomaly in Analysis
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Anomalies
      - Report
  /v1/proxy/clusters/report:
    get:
      summary: Clusters Report
      description: Get Clusters report
      operationId: getClustersReportUsingGET
      x-api-path-slug: v1proxyclustersreport-get
      parameters:
      - in: query
        name: analysisId
        description: Analysis Id
      - in: query
        name: dataSourceName
        description: Data Source name
      - in: query
        name: filterOnlyUsedToCluster
        description: Filter Anomalies used to set create Clusters
      - in: query
        name: fromAnomaly
        description: Filter from Anomaly in Analysis
      - in: query
        name: toAnomaly
        description: Filter to Anomaly in Analysis
      - in: query
        name: withMinClusterSize
        description: Get only Clusters with minimum size
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Clusters
      - Report
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---