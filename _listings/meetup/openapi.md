---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  description: the-meetup-api-provides-simple-restful-http-and-streaming-interfaces-for-exploring-and-interacting-meetup-platform-from-your-own-apps--the-api-is-a-set-of-core-methods-and-a-common-request-format--these-are-combined-to-form-a-url-that-returns-the-information-you-want--
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
---