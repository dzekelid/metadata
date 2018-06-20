---
name: HHS Media Services
x-slug: hhs-media-services
description: Use this API platform to create sites with text and multimedia content
  for syndication. CDC, FDA, HHS, and NIH have built syndication sites using this
  platform, which is available in Java and .NET.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Metadata
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/hhs-media-services/apis.md
specificationVersion: "0.14"
apis:
- name: HHS Media Services Get Youtube metadata for MediaItem
  x-api-slug: hhs-media-services
  description: Returns the Youtube metadata, where applicable, for the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/{id}/youtubeMetaData.json
  tags: Resources,Media,Id,YoutubeMetaData
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/hhs-media-services/resourcesmediaidyoutubemetadata-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/hhs-media-services/resourcesmediaidyoutubemetadata-json-get-openapi.md
- name: HHS Media Services
  x-api-slug: hhs-media-services
  description: Use this API platform to create sites with text and multimedia content
    for syndication. CDC, FDA, HHS, and NIH have built syndication sites using this
    platform, which is available in Java and .NET.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Metadata
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/hhs-media-services/openapi.md
x-common:
- type: x-website
  url: https://api.digitalmedia.hhs.gov/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---