{
  "info": {
    "name": "PayJunction Get Transactions Receipts Latest Thermal",
    "_postman_id": "1a5d4045-3bbb-4215-9301-d692e87b85ec",
    "description": "Get the most recent version of the thermal receipt HTML Document",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Customers",
      "item": [
        {
          "id": "c61177dc-257c-42e0-9985-49911047afef",
          "name": "CustomersGet",
          "request": {
            "url": "http://example.com/customers?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "Gets a list of 15 customers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ee4c0f6-ba55-4038-a33c-19cf594e2e58"
            }
          ]
        },
        {
          "id": "3bfecaec-c178-4320-a7f8-10540dc3d7a5",
          "name": "CustomersByCustomerIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId"
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "/customers/{customerid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b89ff6d-3aa6-4401-819b-3ec0d5c4d842"
            }
          ]
        },
        {
          "id": "2c711fd9-598b-42e7-a1b6-69919b1f5ce8",
          "name": "CustomersByCustomerIdPut",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId"
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
                  "key": "companyName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "custom1",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "defaultAddressId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "firstName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "identifier",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "jobTitle",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "lastName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "middleName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "phone",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "phone2",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "website",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "/customers/{customerid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c154c45-95f0-4838-b946-ad6d9c232629"
            }
          ]
        },
        {
          "id": "06c21c9c-9856-49c2-b70b-81573de2385d",
          "name": "CustomersByCustomerIdDelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId"
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
              "mode": "raw"
            },
            "description": "/customers/{customerid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c18b86e8-a404-4f6f-bdba-84e9c5db6d27"
            }
          ]
        },
        {
          "id": "b799ef18-c4f0-46cd-914a-0deae8d19aa9",
          "name": "CustomersPost",
          "request": {
            "url": "http://example.com/customers/",
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
                  "key": "companyName",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 64"
                },
                {
                  "key": "custom1",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 32"
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "Email (1), Max Length 128"
                },
                {
                  "key": "firstName",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 16"
                },
                {
                  "key": "identifier",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 64"
                },
                {
                  "key": "jobTitle",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 32"
                },
                {
                  "key": "lastName",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 32"
                },
                {
                  "key": "middleName",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 32"
                },
                {
                  "key": "phone",
                  "value": "{}",
                  "disabled": false,
                  "description": "Phone Number, Max Length 24, Must contain at least 10 digits"
                },
                {
                  "key": "phone2",
                  "value": "{}",
                  "disabled": false,
                  "description": "Phone Number, Max Length 24, Must contain at least 10 digits"
                },
                {
                  "key": "website",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 128"
                }
              ]
            },
            "description": "Add a new customer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf840095-b101-433f-be61-c23aa3c09a42"
            }
          ]
        },
        {
          "id": "8fc04556-38e1-4ced-9af8-8988b4cc5c69",
          "name": "CustomersNotesByCustomerIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/notes"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "/customers/{customerid}/notes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1afdd5c1-a971-466a-82d0-695d6486609a"
            }
          ]
        },
        {
          "id": "25bc951d-e19c-4afa-9428-8a95abce3ec1",
          "name": "CustomersNotesByCustomerIdPost",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/notes"
              ],
              "variable": [
                {
                  "id": "customerId",
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
                  "key": "note",
                  "value": "{}",
                  "disabled": false,
                  "description": "Max Length 2048"
                }
              ]
            },
            "description": "/customers/{customerid}/notes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb48424a-86db-458d-a6b3-2a784b3c1bfa"
            }
          ]
        },
        {
          "id": "ba99d70b-5d58-4684-9a59-d4ef33c281f3",
          "name": "CustomersNotesByCustomerIdAndNoteIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/notes/:noteId"
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "/customers/{customerid}/notes/{noteid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b22ca7b9-b81b-4f4d-a6e3-56c05bd41b73"
            }
          ]
        },
        {
          "id": "a27f539f-7893-4c52-87e1-de04ea7b75bc",
          "name": "CustomersNotesByCustomerIdAndNoteIdPut",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/notes/:noteId"
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
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
                  "key": "note",
                  "value": "{}",
                  "disabled": false,
                  "description": "Max Length 2048"
                }
              ]
            },
            "description": "/customers/{customerid}/notes/{noteid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3bbdd452-80b2-4539-97c0-1d9a5da8fbff"
            }
          ]
        },
        {
          "id": "b5258de0-7455-4428-8fd4-e6ac4a855045",
          "name": "CustomersNotesByCustomerIdAndNoteIdDelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/notes/:noteId"
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
              "mode": "raw"
            },
            "description": "/customers/{customerid}/notes/{noteid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f4b6ab0-f3a0-4166-910d-efc839e1047f"
            }
          ]
        },
        {
          "id": "f7b994f1-4db1-400e-b7c2-f74865d5875c",
          "name": "CustomersVaultsByCustomerIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/vaults/"
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "Retrieve customer's payment vaults"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e558a92-df98-48a2-92dd-8dcfe1eec00c"
            }
          ]
        },
        {
          "id": "12e69eff-4fd9-4428-b418-2557ff67adb5",
          "name": "CustomersVaultsByCustomerIdAndVaultIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/vaults/:vaultId"
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "vaultId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "/customers/{customerid}/vaults/{vaultid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc8103ce-ca02-4376-84de-86304b0836c5"
            }
          ]
        },
        {
          "id": "d62a69ae-754d-43ab-9b58-2a1d68c761fb",
          "name": "CustomersVaultsByCustomerIdAndVaultIdDelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/vaults/:vaultId"
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "vaultId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
              "mode": "raw"
            },
            "description": "/customers/{customerid}/vaults/{vaultid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43b00b4a-ec00-4667-8033-dd0f43b8cf53"
            }
          ]
        },
        {
          "id": "c342ae7a-e7e2-40d9-a139-e14e369314d0",
          "name": "CustomersVaultsByCustomerIdPost2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/vaults"
              ],
              "variable": [
                {
                  "id": "customerId",
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
                  "key": "address",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "addressId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "cardExpMonth",
                  "value": "{}",
                  "disabled": false,
                  "description": "1-12"
                },
                {
                  "key": "cardExpYear",
                  "value": "{}",
                  "disabled": false,
                  "description": "YYYY, YY"
                },
                {
                  "key": "cardNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": "5105105105105100,5105-1051-0510-5100,5105 1051 0510 5100"
                },
                {
                  "key": "city",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "state",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "zip",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "/customers/{customerid}/vaults (card)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bde3c15-b54a-4993-b818-2732bde91028"
            }
          ]
        },
        {
          "id": "6a22f7da-6fda-445b-8548-1e684d0c6166",
          "name": "CustomersVaultsByCustomerIdAndAchVaultPut",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/vaults/:achVault"
              ],
              "variable": [
                {
                  "id": "achVault",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
                  "key": "achAccountType",
                  "value": "{}",
                  "disabled": false,
                  "description": "CHECKING, SAVINGS"
                },
                {
                  "key": "achType",
                  "value": "{}",
                  "disabled": false,
                  "description": "CCD, PPD, TEL, WEB"
                },
                {
                  "key": "address",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "addressId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "city",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "state",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "zip",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "/customers/{customerid}/vaults/{vaultid} (ach)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d25049d0-1c53-4beb-9ddd-7c34dc085e8f"
            }
          ]
        },
        {
          "id": "ec08b88f-5734-411c-9b36-29e975e90ec6",
          "name": "CustomersVaultsByCustomerIdAndCardVaultPut",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/vaults/:cardVault"
              ],
              "variable": [
                {
                  "id": "cardVault",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
                  "key": "address",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "addressId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "cardExpMonth",
                  "value": "{}",
                  "disabled": false,
                  "description": "1-12"
                },
                {
                  "key": "cardExpYear",
                  "value": "{}",
                  "disabled": false,
                  "description": "YYYY, YY"
                },
                {
                  "key": "city",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "state",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "zip",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "/customers/{customerid}/vaults/{vaultid} (card)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9c9797b-2e93-46a1-b07a-9ddeb9b0e05c"
            }
          ]
        },
        {
          "id": "2372f804-5152-435b-bbc2-0adc4d32bde1",
          "name": "CustomersAddressesByCustomerIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/addresses"
              ],
              "variable": [
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "Gets a list of a customer's addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d2ed897-fb70-4fc4-bcf4-97f3de543e9d"
            }
          ]
        },
        {
          "id": "1a89bfd5-b484-4dd9-a30d-a4c955b69ee6",
          "name": "CustomersAddressesByCustomerIdPost",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/addresses"
              ],
              "variable": [
                {
                  "id": "customerId",
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
                  "key": "address",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 128"
                },
                {
                  "key": "city",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 32"
                },
                {
                  "key": "country",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 32"
                },
                {
                  "key": "state",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 32"
                },
                {
                  "key": "zip",
                  "value": "{}",
                  "disabled": false,
                  "description": "Text, Max Length 16"
                }
              ]
            },
            "description": "/customers/{customerid}/addresses/."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3644771-3d65-4821-9ac7-dcbf0db8b261"
            }
          ]
        },
        {
          "id": "1f00ad03-af82-4f8e-bbab-62c168f1a89e",
          "name": "CustomersAddressesByCustomerIdAndAddressIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/addresses/:addressId"
              ],
              "variable": [
                {
                  "id": "addressId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "/customers/{customerid}/addresses/{addressid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a82f6b01-9786-4192-98db-41f00ef52dd2"
            }
          ]
        },
        {
          "id": "ba5d5119-8703-490d-b6a6-5cd6e6de66ac",
          "name": "CustomersAddressesByCustomerIdAndAddressIdPut",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/addresses/:addressId"
              ],
              "variable": [
                {
                  "id": "addressId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
                  "key": "address",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "city",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "country",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "state",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "zip",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "/customers/{customerid}/addresses/{addressid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "553638c0-b02c-43e6-bacf-24a346c76385"
            }
          ]
        },
        {
          "id": "d37fb247-67e8-4f13-bff3-ed4e079f0b7d",
          "name": "CustomersAddressesByCustomerIdAndAddressIdDelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "customers/:customerId/addresses/:addressId"
              ],
              "variable": [
                {
                  "id": "addressId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
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
              "mode": "raw"
            },
            "description": "/customers/{customerid}/addresses/{addressid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0209d80a-17d6-4bca-92d0-2f57655de995"
            }
          ]
        }
      ]
    },
    {
      "name": "Transactions",
      "item": [
        {
          "id": "8014dfbe-08b7-4015-adf0-b29266313ce6",
          "name": "TransactionsPost6",
          "request": {
            "url": "http://example.com/transactions",
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
                  "key": "action",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "amountBase",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "billingCompanyName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "billingFirstName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "billingLastName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "cardTrack",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "/transactions/ (swiped cc)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8292b00-c8f7-4ae6-96bd-4b298151d37e"
            }
          ]
        },
        {
          "id": "c6fa8e29-a491-4706-84c8-b01e55e409a2",
          "name": "TransactionsGet",
          "request": {
            "url": "http://example.com/transactions/?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "Not Available At Time at Time of Publishing this collection: Get a list of transactions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "779acf84-17e7-4ada-b995-ea47799a47b2"
            }
          ]
        },
        {
          "id": "97bd971c-05ed-4a48-9eeb-b1c6fd698ab4",
          "name": "TransactionsByTransactionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId"
              ],
              "variable": [
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "/transactions/{transactionid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "845b9920-1512-48ec-9475-50d826ceb0e5"
            }
          ]
        },
        {
          "id": "246c3b10-dfa3-418e-adc0-f6b7baf61861",
          "name": "TransactionsByTransactionIdPut",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId"
              ],
              "variable": [
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
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
                  "key": "amountBase",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "amountReject",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "amountShipping",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "amountTax",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "amountTip",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "status",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Update an unsettled transaction"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fcce559-ae0e-44e2-ba98-7f9bb06747bd"
            }
          ]
        },
        {
          "id": "330fb165-1914-4cda-8a6e-ea4b578847f6",
          "name": "TransactionsNotesByTransactionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId/notes"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "Get a list of notes for a transaction"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa49351b-d3af-47ce-a2cf-100abcb7f27d"
            }
          ]
        },
        {
          "id": "f15bccac-0a35-42fb-872d-479b5277e6f7",
          "name": "TransactionsNotesByTransactionIdPost",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId/notes"
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
                  "key": "note",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "/transactions/{transactionid}/notes/."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07e255eb-dcc3-4498-9268-5bb328561c99"
            }
          ]
        },
        {
          "id": "6702fe45-db41-4409-8616-4239a7178b73",
          "name": "TransactionsNotesByTransactionIdAndNoteIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId/notes/:noteId"
              ],
              "variable": [
                {
                  "id": "noteId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "/transactions/{transactionid}/notes/{noteid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39aba090-3c8c-4a85-9183-64c2942e8262"
            }
          ]
        },
        {
          "id": "342ec9d1-0a7c-4916-bdf9-8fa8a8eab3f6",
          "name": "TransactionsNotesByTransactionIdAndNoteIdPut",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId/notes/:noteId"
              ],
              "variable": [
                {
                  "id": "noteId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
                  "key": "note",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "/transactions/{transactionid}/notes/{noteid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd705686-fbe0-49d0-a58d-58f307853a83"
            }
          ]
        },
        {
          "id": "016e6051-af46-4d32-9f60-57bb56839a9c",
          "name": "TransactionsNotesByTransactionIdAndNoteIdDelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId/notes/:noteId"
              ],
              "variable": [
                {
                  "id": "noteId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
              "mode": "raw"
            },
            "description": "/transactions/{transactionid}/notes/{noteid}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "569f6c01-32f4-4cea-adac-2daeb69a9407"
            }
          ]
        },
        {
          "id": "0ce0f6f8-6778-457f-af50-d137d5741c8e",
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
              "id": "d6b0d04c-fa30-4e39-ad88-3e6a39e0d857"
            }
          ]
        },
        {
          "id": "a0893934-587a-48d9-b953-e8b124cf5ad4",
          "name": "TransactionsReceiptsLatestEmailByTransactionIdPost",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId/receipts/latest/email"
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
                  "key": "replyTo",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "requestSignature",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "to",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "/transactions/{transactionid}/receipts/latest/email."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "519585e3-1bd9-4555-b931-a0d0bd4b76c0"
            }
          ]
        },
        {
          "id": "24d882e0-21d4-47e9-9cbd-16e4de72f94e",
          "name": "TransactionsReceiptsByTransactionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId/receipts"
              ],
              "variable": [
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "Get all of the signed receipts for a transaction."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a7c7bf3-a58a-4a1d-9312-3c33b724ea07"
            }
          ]
        },
        {
          "id": "caa62ac3-8e6e-45f2-9ec9-fa9f834fb2cf",
          "name": "TransactionsReceiptsLatestByTransactionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId/receipts/latest"
              ],
              "variable": [
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "Retrieve the most recent version of the receipt."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a23b333-8fcd-454e-a85b-aa257a22e938"
            }
          ]
        },
        {
          "id": "eba9a67e-b9e3-4ac5-9b2a-863ffc304aaa",
          "name": "TransactionsReceiptsLatestThermalByTransactionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transactionId/receipts/latest/thermal"
              ],
              "variable": [
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
              "mode": "raw"
            },
            "description": "Get the most recent version of the thermal receipt HTML Document"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e98b216-504e-4506-956b-19ed3e29d4a0"
            }
          ]
        }
      ]
    }
  ]
}