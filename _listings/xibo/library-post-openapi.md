---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Add Media
  description: Add Media to the Library
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displaygroup/{displayGroupId}/media/assign:
    post:
      summary: Assign one or more Media items to a Display Group
      description: Adds the provided Media to the Display Group
      operationId: displayGroupMediaAssign
      x-api-path-slug: displaygroupdisplaygroupidmediaassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to assign to
      - in: formData
        name: mediaId
        description: The Media Ids to assign
      - in: formData
        name: unassignMediaId
        description: Optional array of Media Id to unassign
      responses:
        200:
          description: OK
      tags:
      - Assign
      - More
      - Media
      - Items
      - To
      - Display
      - Group
  /displaygroup/{displayGroupId}/media/unassign:
    post:
      summary: Unassign one or more Media items from a Display Group
      description: Removes the provided from the Display Group
      operationId: displayGroupMediaUnassign
      x-api-path-slug: displaygroupdisplaygroupidmediaunassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to unassign from
      - in: formData
        name: mediaId
        description: The Media Ids to unassign
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - More
      - Media
      - Items
      - From
      - Display
      - Group
  /library:
    post:
      summary: Add Media
      description: Add Media to the Library
      operationId: libraryAdd
      x-api-path-slug: library-post
      parameters:
      - in: formData
        name: deleteOldRevisions
        description: Flag (0 , 1), to either remove or leave the old file revisions
          (use with oldMediaId)
      - in: formData
        name: files
        description: The Uploaded File
      - in: formData
        name: name
        description: Optional Media Name
      - in: formData
        name: oldMediaId
        description: Id of an existing media file which should be replaced with the
          new upload
      - in: formData
        name: updateInLayouts
        description: Flag (0, 1), set to 1 to update this media in all layouts (use
          with oldMediaId)
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