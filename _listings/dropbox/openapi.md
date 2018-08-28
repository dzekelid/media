swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
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