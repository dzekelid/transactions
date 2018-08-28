{
  "info": {
    "name": "Yapily Get account transactions",
    "_postman_id": "47f26722-73f5-41b6-896a-ad7142be7940",
    "description": "Get account transactions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "7d96ce11-9de6-4b58-90d7-b159203d53f5",
          "name": "getAccountsUsingGET",
          "request": {
            "url": "http://api.yapily.com:443/accounts",
            "method": "GET",
            "header": [
              {
                "key": "consent",
                "value": "{}",
                "description": "Consent Token",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34668427-25ff-4efd-aad5-6ee81b718da5"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "bbacc8c0-64dd-46d8-b996-f7e6b00004ba",
          "name": "getAccountUsingGET",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.yapily.com",
              "path": [
                "accounts/:accountId"
              ],
              "port": "443",
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "consent",
                "value": "{}",
                "description": "Consent Token",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "608adf43-4866-4047-bf89-eda3785b8758"
            }
          ]
        },
        {
          "id": "7788622a-86b9-4ac8-91bb-8b1380f55404",
          "name": "getTransactionsUsingGET",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.yapily.com",
              "path": [
                "accounts/:accountId/transactions"
              ],
              "port": "443",
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "consent",
                "value": "{}",
                "description": "Consent Token",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get account transactions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c22663b7-fc08-4cd4-b50e-3bd658a3f283"
            }
          ]
        }
      ]
    }
  ]
}