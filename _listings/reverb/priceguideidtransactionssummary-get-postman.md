{
  "info": {
    "name": "reverb Get Pricegue Transactions Summary",
    "_postman_id": "3c99b4c8-10d5-483d-a4bf-74ec074ce267",
    "description": "Get a summary of transactions for a given price guide",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Priceguide",
      "item": [
        {
          "id": "007881c4-8ce8-4dc1-9b42-a6a060bd24fd",
          "name": "getPricegueTransactions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "priceguide/:id/transactions"
              ],
              "query": [
                {
                  "key": "condition",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of paginated transactions for a price guide."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61728265-3d41-4e83-ab45-fb43618105b6"
            }
          ]
        },
        {
          "id": "2daff000-76ce-4239-8d11-502b48ff214d",
          "name": "getPricegueTransactionsSummary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "priceguide/:id/transactions/summary"
              ],
              "query": [
                {
                  "key": "condition",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "number_of_months",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a summary of transactions for a given price guide"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c56a2de2-e613-4c6a-9d94-78e431d5d2d2"
            }
          ]
        }
      ]
    }
  ]
}