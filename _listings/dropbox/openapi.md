---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox
  description: the-dropbox-api-allows-you-to-build-the-power-of-dropbox-directly-into-your-app-
  version: "1"
host: api.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media:
    post:
      summary: Add Media
      description: /media
      operationId: media
      x-api-path-slug: media-post
      parameters:
      - in: query
        name: locale
        description: Use to specify language settings for user error messages and
          other language specific text
      responses:
        200:
          description: OK
      tags:
      - Media
---