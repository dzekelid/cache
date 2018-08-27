swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 1
info:
  title: Compute Engine
  description: creates-and-runs-virtual-machines-on-google-cloud-platform-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/urlMaps/{urlMap}/invalidateCache:
    post:
      summary: Invalidate Cache
      description: Initiates a cache invalidation operation, invalidating the specified
        path, scoped to the specified UrlMap.
      operationId: compute.urlMaps.invalidateCache
      x-api-path-slug: projectglobalurlmapsurlmapinvalidatecache-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: urlMap
        description: Name of the UrlMap scoping this request
      responses:
        200:
          description: OK
      tags:
      - Cache