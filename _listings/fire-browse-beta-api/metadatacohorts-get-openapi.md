---
swagger: "2.0"
x-collection-name: Fire Browse Beta API
x-complete: 0
info:
  title: Fire Browse Beta API Translate TCGA cohort abbreviations to full disease
    names.
  description: By default this function returns a table containing all TCGA cohort
    abbreviations and their corresponding disease names.  A subset of that table may
    be obtained by explicitly specifying one or more cohort abbreviations.
  version: 1.1.35 (2016-09-27 10:12:23 6a47e74011281b2aa
host: firebrowse.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Metadata/Centers:
    get:
      summary: Obtain identities of TCGA consortium member centers.
      description: By default this function returns a table of all consortium members
        in TCGA, aka centers; it provides both the HTTP domain and full organizational
        name of each center.  A subset of this table may be obtained by explicitly
        specifying one or more domain names.
      operationId: getMetadataCenters
      x-api-path-slug: metadatacenters-get
      parameters:
      - in: query
        name: center
        description: Narrow search to one or more TCGA centers from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Centers
  /Metadata/ClinicalNames:
    get:
      summary: Retrieve names of all TCGA clinical data elements (CDEs).
      description: Retrieve names of all patient-level clinical data elements (CDES)
        available in TCGA, unioned across all disease cohorts. A CDE will be listed
        here only when it has a value other than NA for at least 1 patient case in
        any disease cohort. For more information on how these CDEs are processed see
        our pipeline documentation.
      operationId: getMetadataClinicalnames
      x-api-path-slug: metadataclinicalnames-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - ClinicalNames
  /Metadata/ClinicalNames_FH:
    get:
      summary: Retrieve names of CDEs normalized by Firehose and selected for analyses.
      description: This service returns the names of patient-level clinical data elements
        (CDEs) that have been normalized by Firehose for use in analyses, unioned
        across all disease cohorts. For more information on how these CDEs are processed,
        see our pipeline documentation.
      operationId: getMetadataClinicalnamesFh
      x-api-path-slug: metadataclinicalnames-fh-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - ClinicalNames
      - FH
  /Metadata/Cohorts:
    get:
      summary: Translate TCGA cohort abbreviations to full disease names.
      description: By default this function returns a table containing all TCGA cohort
        abbreviations and their corresponding disease names.  A subset of that table
        may be obtained by explicitly specifying one or more cohort abbreviations.
      operationId: getMetadataCohorts
      x-api-path-slug: metadatacohorts-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Cohorts
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