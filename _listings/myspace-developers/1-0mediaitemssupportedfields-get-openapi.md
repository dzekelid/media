---
swagger: "2.0"
x-collection-name: MySpace Developers
x-complete: 0
info:
  title: My Space Get Mediaitems Supported Fields
  description: Retrieves all supported fields.
  version: 1.0.0
host: api.myspace.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1.0/mediaitemcomments/{personId}/@self/{albumId}/{mediaItemId}:
    get:
      summary: Get Mediaitemcomments Personid Self Albums Mediaitemid
      description: Retrieves item comments from a specified album.
      operationId: 1.0.mediaitemcomments.personId._self.albumId.mediaItemId.get
      x-api-path-slug: 1-0mediaitemcommentspersonidselfalbumidmediaitemid-get
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album from the group identified by {selector}
          should be returned
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: path
        name: mediaItemId
        description: Indicates which single media item from the album identified by
          {albumId} should be returned
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - Mediaitemcomments
      - People
      - Self
      - AlbumId
      - MediaItemId
  /1.0/mediaItems/@supportedFields:
    get:
      summary: Get Mediaitems Supported Fields
      description: Retrieves all supported fields.
      operationId: 1.0.mediaItems._supportedFields.get
      x-api-path-slug: 1-0mediaitemssupportedfields-get
      parameters:
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - MediaItems
      - Supported
      - Fields
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