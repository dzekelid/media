{
  "info": {
    "name": "Weather Underground Get Satellite Feature Image Media Type Extension",
    "_postman_id": "1f920d9d-73b3-4ee2-90af-e56590e0f02d",
    "description": "Get sattelitefeature image mediatypeextension",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "weather",
      "item": [
        {
          "id": "08d6d766-7eb9-43e0-960a-63682569a828",
          "name": "getSattelitefeatureImageMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                "DefaultParameterValue",
                ":satteliteFeature/image:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
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
            "description": "Get sattelitefeature image mediatypeextension"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d424eefa-3068-4ff4-9c81-02ddf625db73"
            }
          ]
        }
      ]
    }
  ]
}