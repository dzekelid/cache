{
  "info": {
    "name": "Dezrez Retrieves an object stored in the cache system by its {itemKey}",
    "_postman_id": "8d057b36-ee41-4cb6-b77c-082df58cab4e",
    "description": "Retrieves an object stored in the cache system by its {itemkey}.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieves",
      "item": [
        {
          "id": "a536aaeb-391f-4f6f-af0d-964a1cec9d64",
          "name": "Cache_GetObjectByitemKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/cache/:itemKey"
              ],
              "variable": [
                {
                  "id": "itemKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Retrieves an object stored in the cache system by its {itemkey}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5310ab25-6095-4171-bb2c-099851ce0c12"
            }
          ]
        }
      ]
    }
  ]
}