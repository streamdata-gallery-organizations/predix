---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Data Services Get all available aggregations
  version: 1.0.0
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