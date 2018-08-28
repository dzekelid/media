{
  "info": {
    "name": "Weather Underground Get Radar Sattelite Features Query Media Type Extension",
    "_postman_id": "9c78ff2c-302d-4855-86f4-b43a916c3255",
    "description": "Get radarsattelitefeatures q query mediatypeextension",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "weather",
      "item": [
        {
          "id": "6575e6f5-8ed2-4fa1-924d-6a85854bc681",
          "name": "getRadarsattelitefeaturesQQueryMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                "DefaultParameterValue",
                ":radarSatteliteFeatures/q/:query:mediaTypeExtension"
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
            "description": "Get radarsattelitefeatures q query mediatypeextension"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ae4de07-b170-48fa-98c0-08ca202c8358"
            }
          ]
        }
      ]
    }
  ]
}