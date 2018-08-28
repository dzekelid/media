---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Dropbox Core Returns a link directly to a file.
  description: |-
    Returns a link directly to a file.

    Similar to [/shares](https://www.dropbox.com/developers/core/docs#shares). The difference is that this
    bypasses the Dropbox webserver, used to provide a preview of the file, so that you can effectively stream
    the contents of your media. This URL should not be used to display content directly in the browser.

    The `/media` link expires after four hours, allotting enough time to stream files, but not enough to leave
    a connection open indefinitely.
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/{root}/{path}:
    post:
      summary: Returns a link directly to a file.
      description: |-
        Returns a link directly to a file.

        Similar to [/shares](https://www.dropbox.com/developers/core/docs#shares). The difference is that this
        bypasses the Dropbox webserver, used to provide a preview of the file, so that you can effectively stream
        the contents of your media. This URL should not be used to display content directly in the browser.

        The `/media` link expires after four hours, allotting enough time to stream files, but not enough to leave
        a connection open indefinitely.
      operationId: returns-a-link-directly-to-a-filesimilar-to-shareshttpswwwdropboxcomdeveloperscoredocsshares-the-dif
      x-api-path-slug: mediarootpath-post
      parameters:
      - in: formData
        name: locale
        description: Use to specify language settings for user error messages and
          other language specific text
      - in: path
        name: path
        description: The path to the media file you want a direct link to
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Media
      - Root
      - Path
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