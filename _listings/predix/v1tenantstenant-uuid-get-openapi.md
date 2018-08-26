---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Notification Service Get Tenants
  description: Get tenants.
  version: 1.0.0
host: ev-notification-service.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/tenants/{tenant_uuid}:
    get:
      summary: Get Tenants
      description: Get tenants.
      operationId: getV1TenantsTenantUu
      x-api-path-slug: v1tenantstenant-uuid-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
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