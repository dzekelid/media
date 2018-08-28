swagger: "2.0"
x-collection-name: Google Plus
x-complete: 1
info:
  title: Google Plus
  version: 1.0.0
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