{
  "info": {
    "name": "Stripe Get Bitcoin Receivers Receiver Transactions",
    "_postman_id": "b4b0f2a4-3706-4171-b586-092f5d4a6d54",
    "description": "Get Bitcoin, Receivers, Receiver, Transactions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "bitcoin",
      "item": [
        {
          "id": "a092958f-4344-495a-84f0-5a9c2177af47",
          "name": "getBitcoinReceiversReceiverTransactions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "bitcoin/receivers/:receiver/transactions"
              ],
              "query": [
                {
                  "key": "customer",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ending_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starting_after",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "receiver",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Bitcoin, Receivers, Receiver, Transactions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a40d5dc-3083-46ff-9e43-efbd65a6b16c"
            }
          ]
        }
      ]
    }
  ]
}