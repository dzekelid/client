{
  "info": {
    "name": "Entertainment Express Returns a zip file of client SDK.",
    "_postman_id": "3508b8af-4641-497c-8ec6-adeae6a8de07",
    "description": "Generate and download SDK's for using the API.  Requires a subscription key for authorization and a valid client.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SDKs",
      "item": [
        {
          "id": "f4ceb169-e1ec-42bb-b0bb-225253fbfecd",
          "name": "GetSDK",
          "request": {
            "url": {
              "protocol": "http",
              "host": "ee.iva-api.com",
              "path": [
                "SDKs/:Client"
              ],
              "query": [
                {
                  "key": "RedirectToFile",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "Client",
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
            "description": "Generate and download SDK's for using the API.  Requires a subscription key for authorization and a valid client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6de3ac27-2bde-43e1-8ab6-6216c78473fc"
            }
          ]
        }
      ]
    }
  ]
}