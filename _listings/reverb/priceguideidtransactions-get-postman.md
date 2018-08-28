{
  "info": {
    "name": "reverb Get Pricegue Transactions",
    "_postman_id": "07a8edfb-30fb-4460-a9fd-6a3924fdd794",
    "description": "Get a list of paginated transactions for a price guide.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Priceguide",
      "item": [
        {
          "id": "8c25260d-44e1-482a-944c-07e7d4efe207",
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
              "id": "d4bc3e6f-f18a-4507-b592-e70e0b82d5a7"
            }
          ]
        }
      ]
    }
  ]
}