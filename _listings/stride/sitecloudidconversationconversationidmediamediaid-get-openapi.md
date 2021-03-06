---
swagger: "2.0"
x-collection-name: Stride
x-complete: 0
info:
  title: Stride Get a file
  description: Authentication required, with scope participate:conversation
  version: 1.0.0
host: api.atlassian.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation/{conversationId}/media:
    post:
      summary: Upload a file
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationMediaByCloudIdAndConversationIdPost
      x-api-path-slug: sitecloudidconversationconversationidmedia-post
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: query
        name: name
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Media
  /site/{cloudId}/conversation/{conversationId}/media/{mediaId}:
    get:
      summary: Get a file
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationMediaMediaIdByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationidmediamediaid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: path
        name: mediaId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Media
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