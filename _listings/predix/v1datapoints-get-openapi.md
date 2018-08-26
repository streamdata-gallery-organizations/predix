---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Data Services Query Datapoints
  version: 1.0.0
  description: "Both the GET and POST methods can be used to query time series data.
    Use the query API with the GET HTTP method by passing the query JSON as a URL
    query parameter. The advantage of using the GET method is that requests and responses
    can be cached in proxy servers and browsers.  In cases where the query JSON is
    very long and exceeds query parameter length (for some browsers), use POST as
    a convenience method to query the time series API. POST requests have no restrictions
    on data length, however, requests are never cached. The Time Series service API
    is designed this way to support complex, nested time series queries on one or
    more tags and their attributes, with start and end times, along with aggregations
    and filters.Response JSON (Status 200)\n{\n\t\"tags\": [{\n\t\t\"name\": \"ALT_SENSOR\",\n\t\t\"results\":
    [{\n\t\t\t\"filters\": {\n\t\t\t\t\"attributes\": {\n\t\t\t\t\t\"host\": [\n\t\t\t\t\t\t\"test\"\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"measurements\":
    {\n\t\t\t\t\t\"condition\": \"le\",\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t36\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"qualities\":
    {\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t\"3\"\n\t\t\t\t\t]\n\t\t\t\t}\n\t\t\t},\n\t\t\t\"attributes\":
    {\n\t\t\t\t\"host\": [\"test\"]\n\t\t\t},\n\t\t\t\"values\": [\n\t\t\t\t[1449709894000,
    5, 3],\n\t\t\t\t[1449709895000, 7, 3]\n\t\t\t]\n\t\t}],\n\t\t\"stats\": {\n\t\t\t\"rawCount\":
    2\n\t\t}\n\t}]\n}"
host: time-series-service-doc.grc-apps.svc.ice.ge.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/aggregations:
    get:
      summary: Get all available aggregations
      description: |-
        Return all supported aggregations.Response JSON (Status 200){
          "results": [
            {
              "name": "max",
              "type": "Maximum",
              "description": "Returns the maximum value data point for the time range"
            },
            {
              "name": "trendmode",
              "type": "Trend Mode",
              "description": "Returns the maximum and minimum value data point for the time range"
            },
            {
              "name": "count",
              "type": "Count",
              "description": "Returns the number of data points"
            },
            {
              "name": "scale",
              "type": "Scale",
              "description": "Scales each data point by a factor"
            },
            {
              "name": "interpolate",
              "type": "Interpolate",
              "description": "Does linear interpolation for the chosen window"
            },
            {
              "name": "sum",
              "type": "Sum",
              "description": "Adds the data points together"
            },
            {
              "name": "diff",
              "type": "Difference",
              "description": "Returns the difference between successive data points"
            },
            {
              "name": "gaps",
              "type": "Gaps",
              "description": "Marks gaps in data according to sampling rate with a null data point"
            },
            {
              "name": "sampler",
              "type": "Sampler",
              "description": "Returns the sampling rate of change for the data points"
            },
            {
              "name": "div",
              "type": "Divide",
              "description": "Divides each data point by a divisor"
            },
            {
              "name": "min",
              "type": "Minimum",
              "description": "Returns the minimum value data point for the time range"
            },
            {
              "name": "avg",
              "type": "Average",
              "description": "Returns the average of the data point set"
            },
            {
              "name": "least_squares",
              "type": "Least Squares",
              "description": "Returns a best fit line through the data points using the least squares algorithm"
            },
            {
              "name": "percentile",
              "type": "Percentile",
              "description": "Returns the percentile of the data range"
            },
            {
              "name": "dev",
              "type": "Standard Deviation",
              "description": "Returns the standard deviation of the time series"
            },
            {
              "name": "rate",
              "type": "Rate",
              "description": "Returns the rate of change for the data points"
            }
          ]
        }
      operationId: getAggregationNames
      x-api-path-slug: v1aggregations-get
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Available
      - Aggregations
  /v1/datapoints:
    get:
      summary: Query Datapoints
      description: "Both the GET and POST methods can be used to query time series
        data. Use the query API with the GET HTTP method by passing the query JSON
        as a URL query parameter. The advantage of using the GET method is that requests
        and responses can be cached in proxy servers and browsers.  In cases where
        the query JSON is very long and exceeds query parameter length (for some browsers),
        use POST as a convenience method to query the time series API. POST requests
        have no restrictions on data length, however, requests are never cached. The
        Time Series service API is designed this way to support complex, nested time
        series queries on one or more tags and their attributes, with start and end
        times, along with aggregations and filters.Response JSON (Status 200)\n{\n\t\"tags\":
        [{\n\t\t\"name\": \"ALT_SENSOR\",\n\t\t\"results\": [{\n\t\t\t\"filters\":
        {\n\t\t\t\t\"attributes\": {\n\t\t\t\t\t\"host\": [\n\t\t\t\t\t\t\"test\"\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"measurements\":
        {\n\t\t\t\t\t\"condition\": \"le\",\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t36\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"qualities\":
        {\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t\"3\"\n\t\t\t\t\t]\n\t\t\t\t}\n\t\t\t},\n\t\t\t\"attributes\":
        {\n\t\t\t\t\"host\": [\"test\"]\n\t\t\t},\n\t\t\t\"values\": [\n\t\t\t\t[1449709894000,
        5, 3],\n\t\t\t\t[1449709895000, 7, 3]\n\t\t\t]\n\t\t}],\n\t\t\"stats\": {\n\t\t\t\"rawCount\":
        2\n\t\t}\n\t}]\n}"
      operationId: query
      x-api-path-slug: v1datapoints-get
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      - in: query
        name: query
        description: Valid JSON string
      responses:
        200:
          description: Successful response
      tags:
      - Query
      - Datapoints
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