---
swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 0
info:
  title: IDX Broker Delete Wrapper Cache
  description: Delete wrapper cache.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /clients/wrappercache:
    delete:
      summary: Delete Wrapper Cache
      description: Delete wrapper cache.
      operationId: ClientsWrappercacheDelete
      x-api-path-slug: clientswrappercache-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Wrapper
      - Cache
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