swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oembed:
    get:
      summary: oEmbed
      description: oEmbed implementation
      operationId: oembed
      x-api-path-slug: oembed-get
      parameters:
      - in: query
        name: maxwidth
        description: maximum width to display
        type: string
      - in: query
        name: url
        description: url of resource to be embedded
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - oEmbed
      - Media