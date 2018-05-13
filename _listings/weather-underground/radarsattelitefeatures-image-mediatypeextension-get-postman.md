{
  "info": {
    "name": "Weather Underground Get Radar Satellite Features Image Media Type Extension",
    "_postman_id": "00c4fb30-e683-415d-9e8a-0c252a41d3cb",
    "description": "Get radarsattelitefeatures image mediatypeextension",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "weather",
      "item": [
        {
          "id": "3da5e4bf-de83-4362-8c51-8bb256c449f0",
          "name": "getRadarsattelitefeaturesImageMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                "DefaultParameterValue",
                ":radarSatteliteFeatures/image:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "radarSatteliteFeatures",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get radarsattelitefeatures image mediatypeextension"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3729bf33-f7fe-413c-b27c-0e605d56c2e4"
            }
          ]
        }
      ]
    }
  ]
}