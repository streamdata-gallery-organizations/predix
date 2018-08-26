{
  "info": {
    "name": "Predix Data Services Get all available aggregations",
    "_postman_id": "26d4bbc2-c0c4-493e-8d25-bbc15801c727",
    "description": "Return all supported aggregations.Response JSON (Status 200){\n  \"results\": [\n    {\n      \"name\": \"max\",\n      \"type\": \"Maximum\",\n      \"description\": \"Returns the maximum value data point for the time range\"\n    },\n    {\n      \"name\": \"trendmode\",\n      \"type\": \"Trend Mode\",\n      \"description\": \"Returns the maximum and minimum value data point for the time range\"\n    },\n    {\n      \"name\": \"count\",\n      \"type\": \"Count\",\n      \"description\": \"Returns the number of data points\"\n    },\n    {\n      \"name\": \"scale\",\n      \"type\": \"Scale\",\n      \"description\": \"Scales each data point by a factor\"\n    },\n    {\n      \"name\": \"interpolate\",\n      \"type\": \"Interpolate\",\n      \"description\": \"Does linear interpolation for the chosen window\"\n    },\n    {\n      \"name\": \"sum\",\n      \"type\": \"Sum\",\n      \"description\": \"Adds the data points together\"\n    },\n    {\n      \"name\": \"diff\",\n      \"type\": \"Difference\",\n      \"description\": \"Returns the difference between successive data points\"\n    },\n    {\n      \"name\": \"gaps\",\n      \"type\": \"Gaps\",\n      \"description\": \"Marks gaps in data according to sampling rate with a null data point\"\n    },\n    {\n      \"name\": \"sampler\",\n      \"type\": \"Sampler\",\n      \"description\": \"Returns the sampling rate of change for the data points\"\n    },\n    {\n      \"name\": \"div\",\n      \"type\": \"Divide\",\n      \"description\": \"Divides each data point by a divisor\"\n    },\n    {\n      \"name\": \"min\",\n      \"type\": \"Minimum\",\n      \"description\": \"Returns the minimum value data point for the time range\"\n    },\n    {\n      \"name\": \"avg\",\n      \"type\": \"Average\",\n      \"description\": \"Returns the average of the data point set\"\n    },\n    {\n      \"name\": \"least_squares\",\n      \"type\": \"Least Squares\",\n      \"description\": \"Returns a best fit line through the data points using the least squares algorithm\"\n    },\n    {\n      \"name\": \"percentile\",\n      \"type\": \"Percentile\",\n      \"description\": \"Returns the percentile of the data range\"\n    },\n    {\n      \"name\": \"dev\",\n      \"type\": \"Standard Deviation\",\n      \"description\": \"Returns the standard deviation of the time series\"\n    },\n    {\n      \"name\": \"rate\",\n      \"type\": \"Rate\",\n      \"description\": \"Returns the rate of change for the data points\"\n    }\n  ]\n}",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Available",
      "item": [
        {
          "id": "37792eb7-b57c-4be0-8561-e4e9b72b9b24",
          "name": "getAggregationNames",
          "request": {
            "url": "http://time-series-service-doc.grc-apps.svc.ice.ge.com/v1/aggregations",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Predix-Zone-Id",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Return all supported aggregations.Response JSON (Status 200){\n  \"results\": [\n    {\n      \"name\": \"max\",\n      \"type\": \"Maximum\",\n      \"description\": \"Returns the maximum value data point for the time range\"\n    },\n    {\n      \"name\": \"trendmode\",\n      \"type\": \"Trend Mode\",\n      \"description\": \"Returns the maximum and minimum value data point for the time range\"\n    },\n    {\n      \"name\": \"count\",\n      \"type\": \"Count\",\n      \"description\": \"Returns the number of data points\"\n    },\n    {\n      \"name\": \"scale\",\n      \"type\": \"Scale\",\n      \"description\": \"Scales each data point by a factor\"\n    },\n    {\n      \"name\": \"interpolate\",\n      \"type\": \"Interpolate\",\n      \"description\": \"Does linear interpolation for the chosen window\"\n    },\n    {\n      \"name\": \"sum\",\n      \"type\": \"Sum\",\n      \"description\": \"Adds the data points together\"\n    },\n    {\n      \"name\": \"diff\",\n      \"type\": \"Difference\",\n      \"description\": \"Returns the difference between successive data points\"\n    },\n    {\n      \"name\": \"gaps\",\n      \"type\": \"Gaps\",\n      \"description\": \"Marks gaps in data according to sampling rate with a null data point\"\n    },\n    {\n      \"name\": \"sampler\",\n      \"type\": \"Sampler\",\n      \"description\": \"Returns the sampling rate of change for the data points\"\n    },\n    {\n      \"name\": \"div\",\n      \"type\": \"Divide\",\n      \"description\": \"Divides each data point by a divisor\"\n    },\n    {\n      \"name\": \"min\",\n      \"type\": \"Minimum\",\n      \"description\": \"Returns the minimum value data point for the time range\"\n    },\n    {\n      \"name\": \"avg\",\n      \"type\": \"Average\",\n      \"description\": \"Returns the average of the data point set\"\n    },\n    {\n      \"name\": \"least_squares\",\n      \"type\": \"Least Squares\",\n      \"description\": \"Returns a best fit line through the data points using the least squares algorithm\"\n    },\n    {\n      \"name\": \"percentile\",\n      \"type\": \"Percentile\",\n      \"description\": \"Returns the percentile of the data range\"\n    },\n    {\n      \"name\": \"dev\",\n      \"type\": \"Standard Deviation\",\n      \"description\": \"Returns the standard deviation of the time series\"\n    },\n    {\n      \"name\": \"rate\",\n      \"type\": \"Rate\",\n      \"description\": \"Returns the rate of change for the data points\"\n    }\n  ]\n}"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "6cfd70b1-caa8-4f2e-ad7b-ca23f0d5f196"
            }
          ]
        }
      ]
    }
  ]
}