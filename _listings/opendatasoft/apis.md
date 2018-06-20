---
name: OpenDataSoft
x-slug: opendatasoft
description: OpenDataSoft is a cloud-based turnkey platform for data publishing and
  API management. Its interface is intuitively designed to empower anyone, regardless
  of technical skills, to upload easy-to-understand Open Data, or to even share data
  within an admi...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2716-opendatasoft.jpg
x-kinRank: "7"
x-alexaRank: "307560"
tags: Metadata
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/opendatasoft/apis.md
specificationVersion: "0.14"
apis:
- name: OpenDataSoft Get Source Metadata Templates
  x-api-slug: opendatasoft
  description: List of available metadata templates types, each with their endpoints.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2716-opendatasoft.jpg
  humanURL: http://opendatasoft.com
  baseURL: https://public.opendatasoft.com//api/v2//{source}/metadata_templates
  tags: Source,Metadata,Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/opendatasoft/sourcemetadata-templates-get-openapi.md
- name: OpenDataSoft Get Source Metadata Templates Metadata Template Type
  x-api-slug: opendatasoft
  description: List of metadata templates available for this type.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2716-opendatasoft.jpg
  humanURL: http://opendatasoft.com
  baseURL: https://public.opendatasoft.com//api/v2//{source}/metadata_templates/{metadata_template_type}
  tags: Source,Metadata,Templates,Metadata,Template,Type
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/opendatasoft/sourcemetadata-templatesmetadata-template-type-get-openapi.md
- name: OpenDataSoft Get Source Metadata Templates Metadata Template Type Metadata
    Template Name
  x-api-slug: opendatasoft
  description: A single metadata_template
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2716-opendatasoft.jpg
  humanURL: http://opendatasoft.com
  baseURL: https://public.opendatasoft.com//api/v2//{source}/metadata_templates/{metadata_template_type}/{metadata_template_name}
  tags: Source,Metadata,Templates,Metadata,Template,Type,Metadata,Template,Name
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/opendatasoft/sourcemetadata-templatesmetadata-template-typemetadata-template-name-get-openapi.md
- name: OpenDataSoft
  x-api-slug: opendatasoft
  description: OpenDataSoft is a cloud-based turnkey platform for data publishing
    and API management. Its interface is intuitively designed to empower anyone, regardless
    of technical skills, to upload easy-to-understand Open Data, or to even share
    data within an admi...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2716-opendatasoft.jpg
  humanURL: http://opendatasoft.com
  baseURL: https://public.opendatasoft.com//api/v2
  tags: Metadata
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/opendatasoft/openapi.md
x-common:
- type: x-blog
  url: http://www.opendatasoft.com/category/news/
- type: x-crunchbase
  url: https://crunchbase.com/organization/opendatasoft
- type: x-crunchbase
  url: http://www.crunchbase.com/company/opendatasoft
- type: x-email
  url: contact@opendatasoft.com
- type: x-email
  url: cil@opendatasoft.com
- type: x-twitter
  url: https://twitter.com/opendatasoft
- type: x-website
  url: http://opendatasoft.com
- type: x-website
  url: https://www.opendatasoft.com
- type: x-website
  url: http://www.opendatasoft.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---