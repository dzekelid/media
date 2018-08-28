---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Download a MP3 media
  description: Download a MP3 media, endpoint returns application/binary content-type
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media:
    post:
      summary: Create media
      description: 'Uploads media file to account, acceptable media formats: bmp,
        gif, jpg, m4a, mp3, mp4, png, wav'
      operationId: createMedia
      x-api-path-slug: media-post
      parameters:
      - in: formData
        name: file
        description: Binary media file
      - in: formData
        name: name
        description: A name of a media file
      responses:
        200:
          description: OK
      tags:
      - Media
  /media/public/{key}.{extension}:
    get:
      summary: Download media by extension
      description: 'Download a media file. Available types of files: bmp, gif, jpg,
        m4a, mp3, mp4, png, wav. Content type in response depends on ''extension''
        parameter, e.g. image/jpeg, image/png, audio/mp3, etc'
      operationId: getMediaDataByKey
      x-api-path-slug: mediapublickey-extension-get
      parameters:
      - in: path
        name: extension
        description: 'Media file type, available types: bmp, gif, jpg, m4a, mp3, mp4,
          png, wav'
      - in: path
        name: key
        description: A hash-key of a media resource
      responses:
        200:
          description: OK
      tags:
      - Media
      - Public
      - Key.extension
  /media/{id}:
    get:
      summary: Get a specific media
      description: Get media resource by id
      operationId: getMedia
      x-api-path-slug: mediaid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a media resource
      responses:
        200:
          description: OK
      tags:
      - Media
  /media/{id}.{extension}:
    get:
      summary: Download media by extension
      description: 'Download a media file. Available types of files: bmp, gif, jpg,
        m4a, mp3, mp4, png, wav. Content type in response depends on ''extension''
        parameter, e.g. image/jpeg, image/png, audio/mp3, etc'
      operationId: getMediaData
      x-api-path-slug: mediaid-extension-get
      parameters:
      - in: path
        name: extension
        description: Media file type
      - in: path
        name: id
        description: An id of a media resource
      responses:
        200:
          description: OK
      tags:
      - Media
      - Extensions
  /media/{id}/file:
    get:
      summary: Download a MP3 media
      description: Download a MP3 media, endpoint returns application/binary content-type
      operationId: getMediaDataBinary
      x-api-path-slug: mediaidfile-get
      parameters:
      - in: path
        name: id
        description: An id of a media resource
      responses:
        200:
          description: OK
      tags:
      - Media
      - File
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