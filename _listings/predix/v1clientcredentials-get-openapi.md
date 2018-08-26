---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Tenant Management Get tenant credentials
  description: Get tenant credentials .
  version: 1.0.0
host: predix-tms.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/client-credentials:
    get:
      summary: Get tenant credentials
      description: Get tenant credentials .
      operationId: getTenantCredentialsUsingGET
      x-api-path-slug: v1clientcredentials-get
      parameters:
      - in: header
        name: TMS-Zone-Subdomain
      responses:
        200:
          description: Successful response
      tags:
      - Tenant
      - Credentials
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