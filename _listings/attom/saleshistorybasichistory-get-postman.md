{
  "info": {
    "name": "Attom Data Solutions API Returns basic transaction and loan history on a property.",
    "_postman_id": "6a4cce15-c4d5-47de-9b75-30fe03b22bdf",
    "description": "Get the basic transaction and loan history on a property for a specific address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "bf6df61e-3e8e-4692-a1f8-f6ce5209a5c3",
          "name": "getPropertyIdList",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/id?geoid=%7B%7D&maxBeds=%7B%7D&minBeds=%7B%7D&orderby=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a list of property IDs within a specific geography that have a specific number of beds. Use orderby to choose how you want your results sorted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e6fe40b-8856-436d-beda-4cd5685ecab9"
            }
          ]
        },
        {
          "id": "6e701051-5c89-4ca3-b335-d813b26be11c",
          "name": "propertyDetails",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detail?address=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get property details based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9db355ba-67e7-4abb-9f04-27efe1745e5b"
            }
          ]
        },
        {
          "id": "b8d46ddf-edc9-4ad4-9367-b51321d71b91",
          "name": "adressList",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/address?address1=%7B%7D&address2=%7B%7D&orderby=%7B%7D&page=%7B%7D&pagesize=%7B%7D&postalcode=%7B%7D&propertytype=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a list of properties within a zip code. Use propertytype and order by to narrow down your results."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "311841c6-a75d-4b52-8709-8571de040c9a"
            }
          ]
        },
        {
          "id": "aa840114-6c3a-4ada-9c6c-0b89c2d0dd34",
          "name": "propertySnapshot",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/snapshot?cityname=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&maxavmvalue=%7B%7D&maxLotSize1=%7B%7D&maxtaxamt=%7B%7D&minavmvalue=%7B%7D&minLotSize1=%7B%7D&mintaxamt=%7B%7D&orderby=%7B%7D&postalcode=%7B%7D&propertytype=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a list of property snapshots within a specific city that are within a desired size range and a specific property type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "869e0b39-72f9-4213-8450-8b2f82958aa5"
            }
          ]
        },
        {
          "id": "5b02c367-db1b-41d4-b507-e193de9e640f",
          "name": "propertyBasicProfile",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/basicprofile?attomid=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get basic property information and most recent transaction and taxes for a specific attom id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0125de2-2b8a-44f9-b9ae-8798a946943f"
            }
          ]
        },
        {
          "id": "08325afe-3536-468c-abd3-5b5f46016444",
          "name": "propertyExpandedProfile",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/expandedprofile?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a detailed property information and most recent transaction and taxes for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5375374b-73a9-4c5b-9f93-00eb48b7e112"
            }
          ]
        },
        {
          "id": "43da621f-c57e-48ee-9d83-0d0ce5724398",
          "name": "getAllEventsDetailAddress",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/allevents/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "API Security Key",
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
            "description": "Get a detail of all the events on a specific property based on its address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efcced6b-d7b0-4370-9574-9aa0a4b16aca"
            }
          ]
        },
        {
          "id": "11d50e02-82b2-4ccd-bc3e-d27347192b28",
          "name": "propertyDetailsMortage",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailmortgage?address1=%7B%7D&address2=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get property details mortgage based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aad54ced-835e-47b1-9cf9-efbdb6010040"
            }
          ]
        },
        {
          "id": "82e52698-be3e-497c-8eaf-db7281fa4dff",
          "name": "propertyDetailsOwner",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailowner?address1=%7B%7D&address2=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get property details owner based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34c77fa5-99b0-458c-bded-8e0620405a5a"
            }
          ]
        },
        {
          "id": "2dce6a35-d899-49fc-8edc-a47ed6441b03",
          "name": "propertyDetailsMortgageOwner",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailmortgageowner?address1=%7B%7D&address2=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get property details mortgageowner based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3984063d-06b6-442a-b8b4-d8dc8cf042cd"
            }
          ]
        },
        {
          "id": "9b3bd362-ae93-43a0-8a7f-f3ecf543f587",
          "name": "getAssessmentSnapshotTotal",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/assessment/snapshot?address1=%7B%7D&address2=%7B%7D&maxmktttlvalue=%7B%7D&minmktttlvalue=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get snapshots of the properties within a radius of a property that have a total market value within a specified range."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "feca6855-f8c0-4cb7-96ed-95a20b48d9ac"
            }
          ]
        },
        {
          "id": "a9d6f8fa-51ca-4861-b5d6-a386b5dd00ab",
          "name": "assessmenDetailPropertyId",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/assessment/detail?postalcode=%7B%7D&propertytype=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get assessment details for properties within a zip code. Use propertytpe to select a specific property type for your search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8d7d9b5-b2ac-421f-836c-8be5da997ac5"
            }
          ]
        },
        {
          "id": "bc09c33b-5a14-4be5-8842-9ef90644f6ef",
          "name": "assessmentHistoryDetailID",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/assessmenthistory/detail?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a full detail of property characteristics and assessment history information for a specific property."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e578222-b8a9-47cd-8966-84ed5eab73bd"
            }
          ]
        },
        {
          "id": "85fb8019-db65-4ea9-ac81-5684eda6406c",
          "name": "avmSnapshotGeoID",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/avm/snapshot?geoid=%7B%7D&maxavmvalue=%7B%7D&minavmvalue=%7B%7D&propertytype=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a list of AVM snapshot records that fall within an Onboard GeoID with a specific value range. Use propertytpe to select a specific property type for your search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "796f78c1-963f-43f7-b0e0-d72132bb458a"
            }
          ]
        },
        {
          "id": "cc257fe7-ceb3-4bf1-9946-7626b1af2aed",
          "name": "avmDetailPostal",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/avm/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get AVM details for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd8963f1-6cb3-4de8-b292-ef3dee2876a6"
            }
          ]
        },
        {
          "id": "edbacfd5-adcb-4221-a763-093cdc5f5947",
          "name": "attomAvmDetail",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/attomavm/detail?attomid=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get Attomized AVM and other property details for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62bdb559-1058-474d-9dbb-7d217eef9fa6"
            }
          ]
        },
        {
          "id": "00205258-6a0f-414e-b8e0-52c3e21a4f2d",
          "name": "getHomeSaleSnapshotsGeoId",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/sale/snapshot?address1=%7B%7D&address2=%7B%7D&endsalesearchdate=%7B%7D&geoid=%7B%7D&maxsaleamt=%7B%7D&minsaleamt=%7B%7D&propertytype=%7B%7D&radius=%7B%7D&startsalesearchdate=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a list of home sale snapshots within a Onboard GeoID that sold within a date range and specified sale amount."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f3c80c1-d1df-4517-a12e-b91dc9ce549d"
            }
          ]
        },
        {
          "id": "a3741c7c-25d3-4df1-bc42-b0151cc3cdde",
          "name": "getSaleDetailPostal",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/sale/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get sales information for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66b496f7-cd6a-40e9-a093-82c1c52cfaa3"
            }
          ]
        },
        {
          "id": "6c2bf3ef-9b27-4014-929c-ed770c7c2c39",
          "name": "getSaleHistorySnapshotPropertyId",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/saleshistory/snapshot?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a sales history snapshot of a property based on an Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9dd3759e-ceae-4d9e-b512-01d27c405aba"
            }
          ]
        },
        {
          "id": "e27cbb25-c6d0-4ef7-9c34-a9ae890c543d",
          "name": "saleHistoryBasicHistory",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/saleshistory/basichistory?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get the basic transaction and loan history on a property for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bddaff97-5378-4642-b647-5c68cba76ddd"
            }
          ]
        }
      ]
    },
    {
      "name": "Return",
      "item": [
        {
          "id": "57353e52-f5ee-4227-b1ef-479945d7b8d6",
          "name": "propertyDetailsWithSchools",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailwithschools?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Search for a property to have the property details returned, along with the schools in the associated attendance zones."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21e4d43e-fee6-4d3c-8180-2c5366b93c63"
            }
          ]
        },
        {
          "id": "14e6136d-0422-4251-b1a8-e2371eb3f363",
          "name": "propertySchoolSnapshot",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/school/snapshot?filetypetext=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Search for all schools that are located within a given radius around a given latitude and longitude."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33450f73-2d4f-4f59-90c5-97849eae9975"
            }
          ]
        },
        {
          "id": "d2b4a365-79fb-4da4-8b53-88c9276e025e",
          "name": "propertyDetails",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/school/detail?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Search by school ID to return all of the available details about a school"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d50c6d2f-2226-4c3c-9c6f-db293d743059"
            }
          ]
        },
        {
          "id": "4c9a4536-1df7-4522-9449-3416b370ca8a",
          "name": "propertySchoolDistrictDetail",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/school/districtdetail?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Search by district number to return all of the available details about a school district"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee1bdd8d-4e28-4b94-888f-834911ac4473"
            }
          ]
        }
      ]
    }
  ]
}