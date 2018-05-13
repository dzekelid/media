{
  "info": {
    "name": "Weather Underground Get Radar Feature Query Media Type Extension",
    "_postman_id": "8a65dd62-f6f4-44ea-8913-3581d90435e6",
    "description": "Get radarfeature q query mediatypeextension",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "weather",
      "item": [
        {
          "id": "cdc85631-5a94-4dec-989a-679fc3e492e2",
          "name": "getRadarfeatureQQueryMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                "DefaultParameterValue",
                ":radarFeature/q/:query:mediaTypeExtension"
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
            "description": "Get radarfeature q query mediatypeextension"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "032ae772-9bd5-4e0d-baf6-6c9cd36bb53f"
            }
          ]
        }
      ]
    }
  ]
}