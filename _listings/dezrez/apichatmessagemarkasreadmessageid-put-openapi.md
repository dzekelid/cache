---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez This will update the cache with a new timestamp for when this chat
    message was last read.
  version: 1.0.0
  description: This will update the cache with a new timestamp for when this chat
    message was last read..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/cache/{itemKey}:
    get:
      summary: Retrieves an object stored in the cache system by its {itemKey}
      description: Retrieves an object stored in the cache system by its {itemkey}.
      operationId: Cache_GetObjectByitemKey
      x-api-path-slug: apicacheitemkey-get
      parameters:
      - in: path
        name: itemKey
        description: The item key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - Object
      - Stored
      - In
      - Cache
      - System
      - By
      - Its
      - ItemKey
    put:
      summary: Stores the {objectToPersist} in the cache subsystem.
      description: Stores the {objecttopersist} in the cache subsystem..
      operationId: Cache_SetObjectByobjectToPersistByitemKeyBytimeToLive
      x-api-path-slug: apicacheitemkey-put
      parameters:
      - in: path
        name: itemKey
        description: The item key
      - in: body
        name: objectToPersist
        description: The object to persist
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: timeToLive
        description: The time to live
      responses:
        200:
          description: OK
      tags:
      - Stores
      - ObjectToPersist
      - In
      - Cache
      - Subsystem
  /api/cache/List/{listKey}:
    get:
      summary: Retrieves a list of objects stored in the cache system by its {listKey}
      description: Retrieves a list of objects stored in the cache system by its {listkey}.
      operationId: Cache_GetListBylistKey
      x-api-path-slug: apicachelistlistkey-get
      parameters:
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - List
      - Of
      - Objects
      - Stored
      - In
      - Cache
      - System
      - By
      - Its
      - ListKey
  /api/chat/message/markasread/{messageId}:
    put:
      summary: This will update the cache with a new timestamp for when this chat
        message was last read.
      description: This will update the cache with a new timestamp for when this chat
        message was last read..
      operationId: Chat_MarkMessageAsReadBymessageId
      x-api-path-slug: apichatmessagemarkasreadmessageid-put
      parameters:
      - in: path
        name: messageId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - This
      - Will
      - Update
      - Cache
      - New
      - Timestampwhen
      - This
      - Chat
      - Message
      - Was
      - Last
      - Read
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