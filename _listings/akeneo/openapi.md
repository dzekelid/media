swagger: "2.0"
x-collection-name: Akeneo
x-complete: 1
info:
  title: Official Akeneo PIM API
  description: the-akeneo-api-brought-to-youfind-out-how-this-postman-collection-works-by-visiting-httpapi-akeneo-com
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/media-files/d/d/b/6/ddb6ad393f81503b6be7380785e3b32bbd28cd08_test.png:
    get:
      summary: media
      description: Assuming that the given code is the code of an existing media file
      operationId: RestV1MediaFilesDDB6Ddb6ad393f81503b6be7380785e3b32bbd28cd08TestPngGet
      x-api-path-slug: restv1mediafilesddb6ddb6ad393f81503b6be7380785e3b32bbd28cd08-test-png-get
      responses:
        200:
          description: OK
      tags:
      - Media
  /rest/v1/media-files:
    post:
      summary: media
      description: Assuming that the given identifier is the identifier of an existing
        product and that the given attribute code exists
      operationId: RestV1MediaFilesPost
      x-api-path-slug: restv1mediafiles-post
      parameters:
      - in: header
        name: Content-Type
      - in: formData
        name: file
      - in: formData
        name: product
      responses:
        200:
          description: OK
      tags:
      - Media