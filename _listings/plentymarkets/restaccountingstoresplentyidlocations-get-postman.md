{
  "info": {
    "name": "Plentymarkets List accounting locations of a client",
    "_postman_id": "46ffb05e-22fb-4090-b15e-e1af7a947586",
    "description": "Lists accounting locations of a client. The plenty ID of the client must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "dffec9b2-7145-406b-9700-2fedfc11dbb0",
          "name": "getRestAccountingStoresLocations",
          "request": {
            "url": "http://example.com/rest/accounting/stores/locations",
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
            "description": "List all accounting locations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "105cb647-8fe3-4471-afb7-38a723d85b03"
            }
          ]
        },
        {
          "id": "c52c5a29-6db0-4676-8cff-5e1c06d86085",
          "name": "getRestAccountingStoresPlentyLocations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/stores/:plentyId/locations"
              ],
              "query": [
                {
                  "key": "locationId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "plentyId",
                  "value": "{}",
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
            "description": "Lists accounting locations of a client. The plenty ID of the client must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3b1f91b-d9b1-458c-aeb1-69cb8b1067bf"
            }
          ]
        }
      ]
    }
  ]
}