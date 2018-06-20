---
swagger: "2.0"
x-collection-name: OpenDataSoft
x-complete: 0
info:
  title: OpenDataSoft Get Source Metadata Templates Metadata Template Type
  description: List of metadata templates available for this type.
  version: 2.1.0
host: public.opendatasoft.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{source}/metadata_templates:
    get:
      summary: Get Source Metadata Templates
      description: List of available metadata templates types, each with their endpoints.
      operationId: getMetadataTemplatesTypes
      x-api-path-slug: sourcemetadata-templates-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Metadata
      - Templates
  /{source}/metadata_templates/{metadata_template_type}:
    get:
      summary: Get Source Metadata Templates Metadata Template Type
      description: List of metadata templates available for this type.
      operationId: getMetadataTemplatesType
      x-api-path-slug: sourcemetadata-templatesmetadata-template-type-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Metadata
      - Templates
      - Metadata
      - Template
      - Type
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