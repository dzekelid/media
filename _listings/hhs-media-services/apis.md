---
name: HHS Media Services
x-slug: hhs-media-services
description: Use this API platform to create sites with text and multimedia content
  for syndication. CDC, FDA, HHS, and NIH have built syndication sites using this
  platform, which is available in Java and .NET.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Media
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/apis.md
specificationVersion: "0.14"
apis:
- name: HHS Media Services - Get MediaItems by Campaign ID
  x-api-slug: resourcescampaignsidmedia-json-get
  description: Returns the list of MediaItems for the Campaign identified by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcescampaignsidmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcescampaignsidmedia-json-get-openapi.md
- name: HHS Media Services - Get MediaItems
  x-api-slug: resourcesmedia-json-get
  description: Returns the list of MediaItems matching the specified query parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmedia-json-get-openapi.md
- name: HHS Media Services - Get the list of featured content in the syndication system
  x-api-slug: resourcesmediafeatured-json-get
  description: Get the list of featured content in the syndication system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediafeatured-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediafeatured-json-get-openapi.md
- name: HHS Media Services - Get MediaItems by popularity
  x-api-slug: resourcesmediamostpopularmedia-json-get
  description: Returns the list of MediaItems with the highest ratings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediamostpopularmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediamostpopularmedia-json-get-openapi.md
- name: HHS Media Services - Get MediaItems by search query
  x-api-slug: resourcesmediasearchresults-json-get
  description: Returns the list of MediaItems matching the search query 'q'.The search
    query 'q' is a Lucene query.The syntax for a Lucene query can be found here
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediasearchresults-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediasearchresults-json-get-openapi.md
- name: HHS Media Services - Get MediaItem by ID
  x-api-slug: resourcesmediaid-json-get
  description: Returns the MediaItem identified by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaid-json-get-openapi.md
- name: HHS Media Services - Get content for MediaItem
  x-api-slug: resourcesmediaidcontent-get
  description: Returns the raw content (html, image, etc...) for the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidcontent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidcontent-get-openapi.md
- name: HHS Media Services - Get embed code for MediaItem
  x-api-slug: resourcesmediaidembed-json-get
  description: Returns the javascript or iframe embed code for the MediaItem identified
    by 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidembed-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidembed-json-get-openapi.md
- name: HHS Media Services - Get JPG preview for MediaItem
  x-api-slug: resourcesmediaidpreview-jpg-get
  description: Returns the JPG preview, where applicable, for the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidpreview-jpg-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidpreview-jpg-get-openapi.md
- name: HHS Media Services - Get Ratings for MediaItem
  x-api-slug: resourcesmediaidratings-json-get
  description: Get the Ratings (number of 'likes') for the MediaItem identified by
    the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidratings-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidratings-json-get-openapi.md
- name: HHS Media Services - Get related MediaItems by ID
  x-api-slug: resourcesmediaidrelatedmedia-json-get
  description: Returns the list of MediaItems related to the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidrelatedmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidrelatedmedia-json-get-openapi.md
- name: HHS Media Services - Get syndicated content for MediaItem
  x-api-slug: resourcesmediaidsyndicate-json-get
  description: Returns the syndicated content for a given MediaItem in the specified
    'format' (HTML or JSON).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidsyndicate-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidsyndicate-json-get-openapi.md
- name: HHS Media Services - Get JPG thumbnail for MediaItem
  x-api-slug: resourcesmediaidthumbnail-jpg-get
  description: Returns the JPG thumbnail, where applicable, for the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidthumbnail-jpg-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidthumbnail-jpg-get-openapi.md
- name: HHS Media Services - Get Youtube metadata for MediaItem
  x-api-slug: resourcesmediaidyoutubemetadata-json-get
  description: Returns the Youtube metadata, where applicable, for the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidyoutubemetadata-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcesmediaidyoutubemetadata-json-get-openapi.md
- name: HHS Media Services - Get MediaItems for Tag
  x-api-slug: resourcestagsidmedia-json-get
  description: Returns the list of MediaItems associated with the Tag identified by
    the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Media, API Provider, Videos, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcestagsidmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/media/master/_listings/hhs-media-services/resourcestagsidmedia-json-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://hewlett.packard.enterprise.hpe.api.gallery.streamdata.io
- type: x-api-stack
  url: http://hhs.media.services.stack.network
- type: x-website
  url: https://api.digitalmedia.hhs.gov/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---