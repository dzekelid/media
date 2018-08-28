---
swagger: "2.0"
x-collection-name: Google Plus
x-complete: 0
info:
  title: Google Plus Add Media To Collection
  version: 1.0.0
  description: Add a new media item to an album. The current upload size limitations
    are 36MB for a photo and 1GB for a video. Uploads do not count against quota if
    photos are less than 2048 pixels on their longest side or videos are less than
    15 minutes in length.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /people/{userId}/media/{collection}:
    post:
      summary: Add Media To Collection
      description: Add a new media item to an album. The current upload size limitations
        are 36MB for a photo and 1GB for a video. Uploads do not count against quota
        if photos are less than 2048 pixels on their longest side or videos are less
        than 15 minutes in length.
      operationId: plusDomains.media.insert
      x-api-path-slug: peopleuseridmediacollection-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collection
      - in: path
        name: userId
        description: The ID of the user to create the activity on behalf of
      responses:
        200:
          description: OK
      tags:
      - Media
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