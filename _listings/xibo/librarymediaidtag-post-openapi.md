---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Tag Media
  description: Tag a Media with one or more tags
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
  /library/{mediaId}:
    put:
      summary: Edit Media
      description: Edit a Media Item in the Library
      operationId: libraryEdit
      x-api-path-slug: librarymediaid-put
      parameters:
      - in: formData
        name: duration
        description: The duration in seconds for this Media Item
      - in: path
        name: mediaId
        description: The Media ID to Edit
      - in: formData
        name: name
        description: Media Item Name
      - in: formData
        name: retired
        description: Flag indicating if this media is retired
      - in: formData
        name: tags
        description: Comma separated list of Tags
      - in: formData
        name: updateInLayouts
        description: Flag indicating whether to update the duration in all Layouts
          the Media is assigned to
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Media
    delete:
      summary: Delete Media
      description: Delete Media from the Library
      operationId: libraryDelete
      x-api-path-slug: librarymediaid-delete
      parameters:
      - in: formData
        name: forceDelete
        description: If the media item has been used should it be force removed from
          items that uses it?
      - in: path
        name: mediaId
        description: The Media ID to Delete
      responses:
        200:
          description: OK
      tags:
      - Media
  /library/download/{mediaId}/{type}:
    get:
      summary: Download Media
      description: Download a Media file from the Library
      operationId: libraryDownload
      x-api-path-slug: librarydownloadmediaidtype-get
      parameters:
      - in: path
        name: mediaId
        description: The Media ID to Download
      - in: path
        name: type
        description: The Module Type of the Download
      responses:
        200:
          description: OK
      tags:
      - Download
      - Media
  /library/{mediaId}/tag:
    post:
      summary: Tag Media
      description: Tag a Media with one or more tags
      operationId: mediaTag
      x-api-path-slug: librarymediaidtag-post
      parameters:
      - in: path
        name: mediaId
        description: The Media Id to Tag
      - in: formData
        name: tag
        description: An array of tags
      responses:
        200:
          description: OK
      tags:
      - Tag
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