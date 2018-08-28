{
  "info": {
    "name": "PayJunction Post Transactions Signature Capture",
    "_postman_id": "90f8f229-c948-473c-946b-a83c0616f6b8",
    "description": "Capture a signature using the scriptel signature capture",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Transactions",
      "item": [
        {
          "id": "c770b0b9-d453-4910-8e53-7a5f1dab3c6c",
          "name": "TransactionsSignatureCaptureByTransactionIdPost",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId/signature/capture"
              ],
              "variable": [
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "X-PJ-Application-Key",
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
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "signature",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Capture a signature using the scriptel signature capture"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdc32cb9-abf4-456d-a3db-828d07dceb94"
            }
          ]
        }
      ]
    }
  ]
}