{
  "info": {
    "name": "IDX Broker Delete Wrapper Cache",
    "_postman_id": "c8d6f020-8918-4707-b951-9d0c3edd2993",
    "description": "Delete wrapper cache.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Wrapper",
      "item": [
        {
          "id": "d057936d-351b-494d-b51d-97afda3cc035",
          "name": "ClientsWrappercacheDelete",
          "request": {
            "url": "http://example.com/clients/wrappercache",
            "method": "DELETE",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
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
                "key": "outputtype",
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
            "description": "Delete wrapper cache."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "344d55a3-e1e6-4a2f-8156-9b69dcc424ae"
            }
          ]
        }
      ]
    }
  ]
}