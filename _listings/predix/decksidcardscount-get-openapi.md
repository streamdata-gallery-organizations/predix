---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Views Counts cards of Deck.
  version: 1.0.0
  description: Counts cards of deck..
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /decks/{id}/tags/{fk}:
    delete:
      summary: Delete a related item by id for tags.
      description: Delete a related item by id for tags..
      operationId: deleteDecksTagsFk
      x-api-path-slug: decksidtagsfk-delete
      parameters:
      - in: path
        name: fk
        description: Foreign key for tags
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Related
      - Item
      - By
      - Idtags
  /decks/{id}/cards:
    get:
      summary: Queries cards of Deck.
      description: Queries cards of deck..
      operationId: getDecksCards
      x-api-path-slug: decksidcards-get
      parameters:
      - in: query
        name: filter
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Queries
      - Cards
      - Of
      - Deck
  /decks/{id}/cards/count:
    get:
      summary: Counts cards of Deck.
      description: Counts cards of deck..
      operationId: getDecksCardsCount
      x-api-path-slug: decksidcardscount-get
      parameters:
      - in: path
        name: id
        description: PersistedModel id
      - in: query
        name: where
        description: Criteria to match Deck instances
      responses:
        200:
          description: OK
      tags:
      - Counts
      - Cards
      - Of
      - Deck
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