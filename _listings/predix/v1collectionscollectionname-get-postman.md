{
  "info": {
    "name": "Predix Intelligent Mapping Return all data for a collection",
    "_postman_id": "f099c001-1f23-477b-88bd-c5bc61897c67",
    "description": "Returns the full GeoJSON FeatureCollection uploaded for this collection.\nAll GeoJSON Features will be as originally uploaded with the addition of\na featureId attribute that uniquely identifies the feature across all\nyour collections.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "5e1788e2-330e-47f3-baf7-284a2708fa41",
          "name": "returns-an-array-containing-the-names-of-all-data-collections-for-thespecified-customer",
          "request": {
            "url": "{{default}}/v1/collections?No Name=%7B%7D",
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
            "description": "Returns an array containing the names of all data collections for the\nspecified customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e0161fc-027c-40e8-a9aa-21e643000e1e"
            }
          ]
        }
      ]
    },
    {
      "name": "Return",
      "item": [
        {
          "id": "f4cfe703-e17a-4400-80f9-9b3054fa6f53",
          "name": "returns-the-full-geojson-featurecollection-uploaded-for-this-collectionall-geojson-features-will-be-",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v1/collections/:collectionName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collectionName",
                  "value": "collectionName",
                  "type": "string"
                }
              ]
            },
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
            "description": "Returns the full GeoJSON FeatureCollection uploaded for this collection.\nAll GeoJSON Features will be as originally uploaded with the addition of\na featureId attribute that uniquely identifies the feature across all\nyour collections."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5407f08-4f4d-44eb-ab04-68ca2b294e1d"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/"
    }
  ]
}