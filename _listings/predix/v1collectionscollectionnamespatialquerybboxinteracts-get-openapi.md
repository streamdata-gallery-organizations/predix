---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Dynamic Mapping Returns collection assets in specified bounding box
  description: |-
    Returns all assets in the specified collection whose latest location exist within the specified bounding box.
    The bounding box is defined by two coordinates in the EPSG:4326 (WGS84) (for further details see
    http://epsg.io/4326):
    * left (longitude), bottom (latitude)
    * right (longitude), top (latitude)
    The results can be filtered by including key and value pairs to match in location meta data.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/collections:
    get:
      summary: List all asset collections for a customer
      description: |-
        Returns an array containing the names of all asset collections for the
        specified customer.
      operationId: returns-an-array-containing-the-names-of-all-asset-collections-for-thespecified-customer
      x-api-path-slug: v1collections-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - List
      - ""
      - Asset
      - Collectionsa
      - Customer
  /v1/collections/{collectionName}:
    get:
      summary: Return all asset ids for a collection
      description: |-
        Returns the collection name and a list of ids of the assets that belong to
        the collection.
      operationId: returns-the-collection-name-and-a-list-of-ids-of-the-assets-that-belong-tothe-collection
      x-api-path-slug: v1collectionscollectionname-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Return
      - ""
      - Asset
      - Idsa
      - Collection
    delete:
      summary: Delete a collection
      description: |-
        Delete the asset collection specified by the collection name. Any associated asset and asset location data
        are also deleted
      operationId: delete-the-asset-collection-specified-by-the-collection-name-any-associated-asset-and-asset-location
      x-api-path-slug: v1collectionscollectionname-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Collection
  /v1/collections/{collectionName}/spatial-query/bbox-interacts:
    get:
      summary: Returns collection assets in specified bounding box
      description: |-
        Returns all assets in the specified collection whose latest location exist within the specified bounding box.
        The bounding box is defined by two coordinates in the EPSG:4326 (WGS84) (for further details see
        http://epsg.io/4326):
        * left (longitude), bottom (latitude)
        * right (longitude), top (latitude)
        The results can be filtered by including key and value pairs to match in location meta data.
      operationId: returns-all-assets-in-the-specified-collection-whose-latest-location-exist-within-the-specified-boun
      x-api-path-slug: v1collectionscollectionnamespatialquerybboxinteracts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Returns
      - Collection
      - Assets
      - In
      - Specified
      - Bounding
      - Box
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