---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Enterprise Connect Get EC Gateway settings
  description: Get your EC Gateway settings details
  version: 1.0.0
host: ec-predix-service-osaka.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/settings:
    get:
      summary: Get EC Gateway settings
      description: Get your EC Gateway settings details
      operationId: get-your-ec-gateway-settings-details
      x-api-path-slug: apisettings-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer *your_token
      - in: header
        name: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - EC
      - Gateway
      - Settings
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