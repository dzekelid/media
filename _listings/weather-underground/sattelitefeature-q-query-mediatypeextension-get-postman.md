{
  "info": {
    "name": "Weather Underground Get Satellite Featuer Query Media Type Extension",
    "_postman_id": "bdb35365-49e5-400b-85e6-e61ba3a58f72",
    "description": "Get sattelitefeature q query mediatypeextension",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "weather",
      "item": [
        {
          "id": "021ef7e3-e2d6-49d7-b8d9-605fb27ec730",
          "name": "getSattelitefeatureQQueryMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                "DefaultParameterValue",
                ":satteliteFeature/q/:query:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "query",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "satteliteFeature",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get sattelitefeature q query mediatypeextension"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d076f6d-96ef-4713-9002-0ee39c135eeb"
            }
          ]
        }
      ]
    }
  ]
}