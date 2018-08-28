---
name: Xibo
x-slug: xibo
description: Xibo Digital Signage is a low-cost, high performance solution to launch
  your business, workplace or organisation into the future. Xibo doesn&rsquo;t just
  replicate print media, but actively increases engagement allowing you to deliver
  your message more effectively than ever before.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/xibo-digital-signage-logo.jpeg
x-kinRank: "7"
x-alexaRank: ""
tags: Media
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/apis.md
specificationVersion: "0.14"
apis:
- name: Xibo API - Assign one or more Media items to a Display Group
  x-api-slug: displaygroupdisplaygroupidmediaassign-post
  description: Adds the provided Media to the Display Group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/xibo-digital-signage-logo.jpeg
  humanURL: http://www.xibo.org.uk
  baseURL: https:////api
  tags: Signs, Signage, Display, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/displaygroupdisplaygroupidmediaassign-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/displaygroupdisplaygroupidmediaassign-post-openapi.md
- name: Xibo API - Unassign one or more Media items from a Display Group
  x-api-slug: displaygroupdisplaygroupidmediaunassign-post
  description: Removes the provided from the Display Group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/xibo-digital-signage-logo.jpeg
  humanURL: http://www.xibo.org.uk
  baseURL: https:////api
  tags: Signs, Signage, Display, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/displaygroupdisplaygroupidmediaunassign-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/displaygroupdisplaygroupidmediaunassign-post-openapi.md
- name: Xibo API - Add Media
  x-api-slug: library-post
  description: Add Media to the Library
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/xibo-digital-signage-logo.jpeg
  humanURL: http://www.xibo.org.uk
  baseURL: https:////api
  tags: Signs, Signage, Display, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/library-post-openapi.md
- name: Xibo API - Edit Media
  x-api-slug: librarymediaid-put
  description: Edit a Media Item in the Library
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/xibo-digital-signage-logo.jpeg
  humanURL: http://www.xibo.org.uk
  baseURL: https:////api
  tags: Signs, Signage, Display, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/librarymediaid-put-openapi.md
- name: Xibo API - Delete Media
  x-api-slug: librarymediaid-delete
  description: Delete Media from the Library
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/xibo-digital-signage-logo.jpeg
  humanURL: http://www.xibo.org.uk
  baseURL: https:////api
  tags: Signs, Signage, Display, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/librarymediaid-delete-openapi.md
- name: Xibo API - Download Media
  x-api-slug: librarydownloadmediaidtype-get
  description: Download a Media file from the Library
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/xibo-digital-signage-logo.jpeg
  humanURL: http://www.xibo.org.uk
  baseURL: https:////api
  tags: Signs, Signage, Display, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/librarydownloadmediaidtype-get-openapi.md
- name: Xibo API - Tag Media
  x-api-slug: librarymediaidtag-post
  description: Tag a Media with one or more tags
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/xibo-digital-signage-logo.jpeg
  humanURL: http://www.xibo.org.uk
  baseURL: https:////api
  tags: Signs, Signage, Display, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/librarymediaidtag-post-openapi.md
- name: Xibo API - Untag Media
  x-api-slug: librarymediaiduntag-post
  description: Untag a Media with one or more tags
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/xibo-digital-signage-logo.jpeg
  humanURL: http://www.xibo.org.uk
  baseURL: https:////api
  tags: Signs, Signage, Display, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/xibo/librarymediaiduntag-post-openapi.md
x-common:
- type: x-blog-rss
  url: https://blog.xibo.org.uk/rss/
- type: x-github
  url: https://github.com/xibosignage
- type: x-twitter
  url: https://twitter.com/xibosignage
- type: x-website
  url: http://www.xibo.org.uk
- type: x-api-gallery
  url: http://xero.api.gallery.streamdata.io
- type: x-blog
  url: https://blog.xibo.org.uk/
- type: x-website
  url: https://xibo.org.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---