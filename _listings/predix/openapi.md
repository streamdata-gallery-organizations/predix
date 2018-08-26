---
swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
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
  /decks/{id}/tags:
    get:
      summary: Queries tags of Deck.
      description: Queries tags of deck..
      operationId: getDecksTags
      x-api-path-slug: decksidtags-get
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
      - Tags
      - Of
      - Deck
    post:
      summary: Creates a new instance in tags of this Tag.
      description: Creates a new instance in tags of this tag..
      operationId: postDecksTags
      x-api-path-slug: decksidtags-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Instance
      - In
      - Tags
      - Of
      - This
      - Tag
    delete:
      summary: Deletes all tags of this Deck.
      description: Deletes all tags of this deck..
      operationId: deleteDecksTags
      x-api-path-slug: decksidtags-delete
      parameters:
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Tags
      - Of
      - This
      - Deck
  /decks:
    post:
      summary: Create a new instance of the Deck and persist it.
      description: Create a new instance of the deck and persist it..
      operationId: postDecks
      x-api-path-slug: decks-post
      parameters:
      - in: body
        name: data
        description: Deck instance data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Instance
      - Of
      - Deck
      - Persist
      - It
    get:
      summary: Find all instances of the Deck matched by filter.
      description: Find all instances of the deck matched by filter..
      operationId: getDecks
      x-api-path-slug: decks-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields, where, include, order, offset, and limit
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Instances
      - Of
      - Deck
      - Matched
      - By
      - Filter
  /decks/{id}:
    get:
      summary: Find a Deck instance by id.
      description: Find a deck instance by id..
      operationId: getDecks
      x-api-path-slug: decksid-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields and include
      - in: path
        name: id
        description: Deck id
      responses:
        200:
          description: OK
      tags:
      - Find
      - Deck
      - Instance
      - By
      - Id
    delete:
      summary: Delete a Tag instance by id.
      description: Delete a tag instance by id..
      operationId: deleteDecks
      x-api-path-slug: decksid-delete
      parameters:
      - in: path
        name: id
        description: Deck id
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Instance
      - By
      - Id
    put:
      summary: Update attributes for a Tag instance and persist it.
      description: Update attributes for a tag instance and persist it..
      operationId: putDecks
      x-api-path-slug: decksid-put
      parameters:
      - in: body
        name: data
        description: An object of Deck property name/value pairs
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Attributesa
      - Tag
      - Instance
      - Persist
      - It
  /decks/{id}/cards/ordered:
    get:
      summary: API return deck
      description: Api return deck.
      operationId: getDecksCardsOrdered
      x-api-path-slug: decksidcardsordered-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - API
      - Return
      - Deck
  /decks/{id}/cards/add:
    post:
      summary: Add Cards to Deck
      description: Add cards to deck.
      operationId: postDecksCardsAdd
      x-api-path-slug: decksidcardsadd-post
      parameters:
      - in: body
        name: cardIds
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cards
      - To
      - Deck
  /decks/{id}/cards/remove:
    post:
      summary: Remove Cards from Deck
      description: Remove cards from deck.
      operationId: postDecksCardsRemove
      x-api-path-slug: decksidcardsremove-post
      parameters:
      - in: body
        name: cardIds
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Cards
      - From
      - Deck
  /decks/tags:
    get:
      summary: Get all decks by tags
      description: Get all decks by tags.
      operationId: getDecksTags
      x-api-path-slug: deckstags-get
      parameters:
      - in: query
        name: values
      responses:
        200:
          description: OK
      tags:
      - Decks
      - By
      - Tags
  /decks/bulkCreateCardsAndDecks:
    post:
      summary: Bulk create decks and cards
      description: Bulk create decks and cards.
      operationId: postDecksBulkcreatecardsanddecks
      x-api-path-slug: decksbulkcreatecardsanddecks-post
      parameters:
      - in: body
        name: decks
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Create
      - Decks
      - Cards
  /cards/{id}/tags/{fk}:
    delete:
      summary: Delete a related item by id for tags.
      description: Delete a related item by id for tags..
      operationId: deleteCardsTagsFk
      x-api-path-slug: cardsidtagsfk-delete
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
  /cards/{id}/tags:
    get:
      summary: Queries tags of Card.
      description: Queries tags of card..
      operationId: getCardsTags
      x-api-path-slug: cardsidtags-get
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
      - Tags
      - Of
      - Card
    post:
      summary: Creates a new instance in tags of this Card.
      description: Creates a new instance in tags of this card..
      operationId: postCardsTags
      x-api-path-slug: cardsidtags-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Instance
      - In
      - Tags
      - Of
      - This
      - Card
    delete:
      summary: Deletes all tags of this Card.
      description: Deletes all tags of this card..
      operationId: deleteCardsTags
      x-api-path-slug: cardsidtags-delete
      parameters:
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Tags
      - Of
      - This
      - Card
  /cards:
    post:
      summary: Create a new instance of the Cards and persist it.
      description: Create a new instance of the cards and persist it..
      operationId: postCards
      x-api-path-slug: cards-post
      parameters:
      - in: body
        name: data
        description: Card instance data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Instance
      - Of
      - Cards
      - Persist
      - It
    get:
      summary: Find all instances of the Card matched by filter.
      description: Find all instances of the card matched by filter..
      operationId: getCards
      x-api-path-slug: cards-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields, where, include, order, offset, and limit
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Instances
      - Of
      - Card
      - Matched
      - By
      - Filter
  /cards/count:
    get:
      summary: Counts cards.
      description: Counts cards..
      operationId: getCardsCount
      x-api-path-slug: cardscount-get
      parameters:
      - in: query
        name: where
        description: Criteria to match Card instances
      responses:
        200:
          description: OK
      tags:
      - Counts
      - Cards
  /cards/{id}:
    get:
      summary: Find a Card instance by id.
      description: Find a card instance by id..
      operationId: getCards
      x-api-path-slug: cardsid-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields and include
      - in: path
        name: id
        description: Card id
      responses:
        200:
          description: OK
      tags:
      - Find
      - Card
      - Instance
      - By
      - Id
    delete:
      summary: Delete a Card instance by id.
      description: Delete a card instance by id..
      operationId: deleteCards
      x-api-path-slug: cardsid-delete
      parameters:
      - in: path
        name: id
        description: Card id
      responses:
        200:
          description: OK
      tags:
      - Card
      - Instance
      - By
      - Id
    put:
      summary: Update attributes for a Card instance and persist it.
      description: Update attributes for a card instance and persist it..
      operationId: putCards
      x-api-path-slug: cardsid-put
      parameters:
      - in: body
        name: data
        description: An object of Card property name/value pairs
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Attributesa
      - Card
      - Instance
      - Persist
      - It
  /cards/tags:
    get:
      summary: Get all cards by tags
      description: Get all cards by tags.
      operationId: getCardsTags
      x-api-path-slug: cardstags-get
      parameters:
      - in: query
        name: values
      responses:
        200:
          description: OK
      tags:
      - Cards
      - By
      - Tags
---