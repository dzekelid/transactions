{
  "info": {
    "name": "Stripe Get Bitcoin Transactions",
    "_postman_id": "ba65004e-7a5d-4e5f-92b9-12e445adb8d0",
    "description": "Get Bitcoin, Transactions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "bitcoin",
      "item": [
        {
          "id": "64b24d71-563a-4c9e-8cca-3faa18fc6dc1",
          "name": "getBitcoinTransactions",
          "request": {
            "url": "http://api.stripe.com/v1/bitcoin/transactions?customer=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&receiver=%7B%7D&starting_after=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Bitcoin, Transactions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c50d516d-9c6c-4f14-9cfb-c3363a937663"
            }
          ]
        }
      ]
    }
  ]
}