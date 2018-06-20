---
swagger: "2.0"
x-collection-name: Fire Browse Beta API
x-complete: 1
info:
  title: Fire Browse Beta API
  description: a-simple-and-elegant-way-to-explore-cancer-data
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
  /Metadata/Counts:
    get:
      summary: Retrieve sample counts.
      description: |-
        Returns the aliquot counts for each disease cohort, per sample
        type and data type.  The sample type designation of "Tumor"
        may be used to aggregate the count of all tumor aliquots into
        a single number per disease and data type. See the SampleTypes
        function for a complete description of sample types.
      operationId: getMetadataCounts
      x-api-path-slug: metadatacounts-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: data_type
        description: Narrow search to one or more TCGA data types from the scrollable
          list
      - in: query
        name: date
        description: Select one or more date stamps
      - in: query
        name: format
        description: Format of result
      - in: query
        name: sample_type
        description: Narrow search to one or more TCGA sample types from the scrollable
          list
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: totals
        description: Output an entry providing the totals for each data type
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Counts
  /Metadata/Dates:
    get:
      summary: Retrieve datestamps of all GDAC Firehose standard data and analyses
        runs that have been ingested into FireBrowse.
      description: Retrieve datestamps of all gdac firehose standard data and analyses
        runs that have been ingested into firebrowse..
      operationId: getMetadataDates
      x-api-path-slug: metadatadates-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Dates
  /Metadata/HeartBeat:
    get:
      summary: Simple way to discern whether API server is up and running
      description: Returns a message to indicate that API (server) is up and running,
        or times out if not.
      operationId: getMetadataHeartbeat
      x-api-path-slug: metadataheartbeat-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - HeartBeat
  /Metadata/MAFColNames:
    get:
      summary: Retrieve names of all columns in the mutation annotation files (MAFs)
        served by FireBrowse.
      description: Retrieve the names of all columns in the mutation annotation files
        (MAFs) hosted by FireBrowse.  For more information on the mutation data, and
        how it is processed by Firehose, please consult the pipeline documentation.
      operationId: getMetadataMafcolnames
      x-api-path-slug: metadatamafcolnames-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - MAFColNames
  /Metadata/Patients:
    get:
      summary: Retrieve list of all TCGA patients.
      description: This service returns a list of all TCGA patient barcodes in FireBrowse,
        optionally filtered by disease cohort.  The barcodes are obtained directy
        from the clinical data.
      operationId: getMetadataPatients
      x-api-path-slug: metadatapatients-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Patients
  /Metadata/Platforms:
    get:
      summary: Translate TCGA platform codes to full platform names.
      description: By default this function returns a table of all of the technology
        platforms used to sequence or characterize samples in TCGA--both their short
        platform codes and full names.  A subset of this table may be obtained by
        explicitly specifying one or more platform codes.
      operationId: getMetadataPlatforms
      x-api-path-slug: metadataplatforms-get
      parameters:
      - in: query
        name: format
        description: Format of result
      - in: query
        name: platform
        description: Narrow search to one or more TCGA data generation platforms from
          the scrollable list
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Platforms
  /Metadata/SampleType/Barcode/{TCGA_Barcode}:
    get:
      summary: Given a TCGA barcode, return its short letter sample type code.
      description: Given a tcga barcode, return its short letter sample type code..
      operationId: getMetadataSampletypeBarcodeTcgaBarcode
      x-api-path-slug: metadatasampletypebarcodetcga-barcode-get
      parameters:
      - in: query
        name: format
        description: Format of result
      - in: path
        name: TCGA_Barcode
        description: 'Enter a single TCGA barcode, of any form: e'
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - SampleType
      - Barcode
      - TCGA
      - Barcode
  /Metadata/SampleType/Code/{code}:
    get:
      summary: Translate from numeric to symbolic TCGA sample codes.
      description: Convert a TCGA numeric sample type code (e.g. 01, 02) to its corresponding
        symbolic (short letter) code (e.g. TP, TR).
      operationId: getMetadataSampletypeCodeCode
      x-api-path-slug: metadatasampletypecodecode-get
      parameters:
      - in: path
        name: code
        description: Narrow search to one or more TCGA sample type codes
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - SampleType
      - Code
      - Code
  /Metadata/SampleType/ShortLetterCode/{short_letter_code}:
    get:
      summary: Translate from symbolic to numeric TCGA sample codes.
      description: Convert a TCGA sample type code in symbolic form (or 'short letter
        code' like TP, TR) to its corresponding numeric form (e.g. 01, 02).
      operationId: getMetadataSampletypeShortlettercodeShortLetterCode
      x-api-path-slug: metadatasampletypeshortlettercodeshort-letter-code-get
      parameters:
      - in: query
        name: format
        description: Format of result
      - in: path
        name: short_letter_code
        description: TCGA sample type short letter code(s) (e
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - SampleType
      - ShortLetterCode
      - Short
      - Letter
      - Code
  /Metadata/SampleTypes:
    get:
      summary: Return all TCGA sample type codes, both numeric and symbolic.
      description: Return all tcga sample type codes, both numeric and symbolic..
      operationId: getMetadataSampletypes
      x-api-path-slug: metadatasampletypes-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - SampleTypes
  /Metadata/TSSites:
    get:
      summary: Obtain identities of tissue source sites in TCGA.
      description: By default this function returns a table of all sites which contributed
        source tissue to TCGA, aka TSS's. A subset of this table may be obtained by
        explicitly specifying one or more sites.
      operationId: getMetadataTssites
      x-api-path-slug: metadatatssites-get
      parameters:
      - in: query
        name: format
        description: Format of result
      - in: query
        name: tss_code
        description: Narrow search to one or more TSS codes
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - TSSites
---