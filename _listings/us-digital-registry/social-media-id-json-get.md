---
swagger: "2.0"
info:
  title: U.S. Digital Registry Social Media API Social Media
  description: This returns an agency based on an ID.
  version: 1.0.0
host: usdigitalregistry.digitalgov.gov
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /social_media/{id}.json:
    get:
      summary: Social Media
      description: This returns an agency based on an ID
      operationId: Api::V1::SocialMedia#show
      parameters:
      - in: path
        name: id
        description: ID of the account
      responses:
        200:
          description: OK
      tags:
      - social media
definitions: []
x-collection-name: U.S. Digital Registry
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---