{
  "info": {
    "name": "Weather Underground Get Radar Feature Image Media Type Extension",
    "_postman_id": "f42586a3-ce73-4b25-9294-e9353e10efaf",
    "description": "Get radarfeature image mediatypeextension",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "weather",
      "item": [
        {
          "id": "76cf93b7-69b9-465e-a45d-3d20bba7e995",
          "name": "getRadarfeatureImageMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                "DefaultParameterValue",
                ":radarFeature/image:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "radarFeature",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get radarfeature image mediatypeextension"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e26ae69f-56df-4e9e-938e-b2fb6816315d"
            }
          ]
        }
      ]
    }
  ]
}