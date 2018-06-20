---
name: Fire Browse Beta API
x-slug: fire-browse-beta-api
description: A simple and elegant way to explore cancer data. Sitting above one of
  the deepest and most integratively characterized open cancer datasets in the world.
  Backed by a powerful computational infrastructure, application programming interface
  (API), graphical tools and online reports. With over 80K sample aliquots from 11,000+
  cancer patients, spanning 38 unique disease cohorts.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Metadata
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/apis.md
specificationVersion: "0.14"
apis:
- name: Fire Browse Beta API Obtain identities of TCGA consortium member centers.
  x-api-slug: fire-browse-beta-api
  description: By default this function returns a table of all consortium members
    in TCGA, aka centers; it provides both the HTTP domain and full organizational
    name of each center.  A subset of this table may be obtained by explicitly specifying
    one or more domain names.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/Centers
  tags: Metadata,Centers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatacenters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatacenters-get-openapi.md
- name: Fire Browse Beta API Retrieve names of all TCGA clinical data elements (CDEs).
  x-api-slug: fire-browse-beta-api
  description: Retrieve names of all patient-level clinical data elements (CDES) available
    in TCGA, unioned across all disease cohorts. A CDE will be listed here only when
    it has a value other than NA for at least 1 patient case in any disease cohort.
    For more information on how these CDEs are processed see our pipeline documentation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/ClinicalNames
  tags: Metadata,ClinicalNames
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadataclinicalnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadataclinicalnames-get-openapi.md
- name: Fire Browse Beta API Retrieve names of CDEs normalized by Firehose and selected
    for analyses.
  x-api-slug: fire-browse-beta-api
  description: This service returns the names of patient-level clinical data elements
    (CDEs) that have been normalized by Firehose for use in analyses, unioned across
    all disease cohorts. For more information on how these CDEs are processed, see
    our pipeline documentation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/ClinicalNames_FH
  tags: Metadata,ClinicalNames,FH
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadataclinicalnames-fh-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadataclinicalnames-fh-get-openapi.md
- name: Fire Browse Beta API Translate TCGA cohort abbreviations to full disease names.
  x-api-slug: fire-browse-beta-api
  description: By default this function returns a table containing all TCGA cohort
    abbreviations and their corresponding disease names.  A subset of that table may
    be obtained by explicitly specifying one or more cohort abbreviations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/Cohorts
  tags: Metadata,Cohorts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatacohorts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatacohorts-get-openapi.md
- name: Fire Browse Beta API Retrieve sample counts.
  x-api-slug: fire-browse-beta-api
  description: |-
    Returns the aliquot counts for each disease cohort, per sample
    type and data type.  The sample type designation of "Tumor"
    may be used to aggregate the count of all tumor aliquots into
    a single number per disease and data type. See the SampleTypes
    function for a complete description of sample types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/Counts
  tags: Metadata,Counts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatacounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatacounts-get-openapi.md
- name: Fire Browse Beta API Retrieve datestamps of all GDAC Firehose standard data
    and analyses runs that have been ingested into FireBrowse.
  x-api-slug: fire-browse-beta-api
  description: Retrieve datestamps of all gdac firehose standard data and analyses
    runs that have been ingested into firebrowse..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/Dates
  tags: Metadata,Dates
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatadates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatadates-get-openapi.md
- name: Fire Browse Beta API Simple way to discern whether API server is up and running
  x-api-slug: fire-browse-beta-api
  description: Returns a message to indicate that API (server) is up and running,
    or times out if not.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/HeartBeat
  tags: Metadata,HeartBeat
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadataheartbeat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadataheartbeat-get-openapi.md
- name: Fire Browse Beta API Retrieve names of all columns in the mutation annotation
    files (MAFs) served by FireBrowse.
  x-api-slug: fire-browse-beta-api
  description: Retrieve the names of all columns in the mutation annotation files
    (MAFs) hosted by FireBrowse.  For more information on the mutation data, and how
    it is processed by Firehose, please consult the pipeline documentation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/MAFColNames
  tags: Metadata,MAFColNames
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatamafcolnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatamafcolnames-get-openapi.md
- name: Fire Browse Beta API Retrieve list of all TCGA patients.
  x-api-slug: fire-browse-beta-api
  description: This service returns a list of all TCGA patient barcodes in FireBrowse,
    optionally filtered by disease cohort.  The barcodes are obtained directy from
    the clinical data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/Patients
  tags: Metadata,Patients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatapatients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatapatients-get-openapi.md
- name: Fire Browse Beta API Translate TCGA platform codes to full platform names.
  x-api-slug: fire-browse-beta-api
  description: By default this function returns a table of all of the technology platforms
    used to sequence or characterize samples in TCGA--both their short platform codes
    and full names.  A subset of this table may be obtained by explicitly specifying
    one or more platform codes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/Platforms
  tags: Metadata,Platforms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadataplatforms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadataplatforms-get-openapi.md
- name: Fire Browse Beta API Given a TCGA barcode, return its short letter sample
    type code.
  x-api-slug: fire-browse-beta-api
  description: Given a tcga barcode, return its short letter sample type code..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/SampleType/Barcode/{TCGA_Barcode}
  tags: Metadata,SampleType,Barcode,TCGA,Barcode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatasampletypebarcodetcga-barcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatasampletypebarcodetcga-barcode-get-openapi.md
- name: Fire Browse Beta API Translate from numeric to symbolic TCGA sample codes.
  x-api-slug: fire-browse-beta-api
  description: Convert a TCGA numeric sample type code (e.g. 01, 02) to its corresponding
    symbolic (short letter) code (e.g. TP, TR).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/SampleType/Code/{code}
  tags: Metadata,SampleType,Code,Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatasampletypecodecode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatasampletypecodecode-get-openapi.md
- name: Fire Browse Beta API Translate from symbolic to numeric TCGA sample codes.
  x-api-slug: fire-browse-beta-api
  description: Convert a TCGA sample type code in symbolic form (or 'short letter
    code' like TP, TR) to its corresponding numeric form (e.g. 01, 02).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/SampleType/ShortLetterCode/{short_letter_code}
  tags: Metadata,SampleType,ShortLetterCode,Short,Letter,Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatasampletypeshortlettercodeshort-letter-code-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatasampletypeshortlettercodeshort-letter-code-get-openapi.md
- name: Fire Browse Beta API Return all TCGA sample type codes, both numeric and symbolic.
  x-api-slug: fire-browse-beta-api
  description: Return all tcga sample type codes, both numeric and symbolic..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/SampleTypes
  tags: Metadata,SampleTypes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatasampletypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatasampletypes-get-openapi.md
- name: Fire Browse Beta API Obtain identities of tissue source sites in TCGA.
  x-api-slug: fire-browse-beta-api
  description: By default this function returns a table of all sites which contributed
    source tissue to TCGA, aka TSS's. A subset of this table may be obtained by explicitly
    specifying one or more sites.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1//Metadata/TSSites
  tags: Metadata,TSSites
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatatssites-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/metadatatssites-get-openapi.md
- name: Fire Browse Beta API
  x-api-slug: fire-browse-beta-api
  description: A simple and elegant way to explore cancer data. Sitting above one
    of the deepest and most integratively characterized open cancer datasets in the
    world. Backed by a powerful computational infrastructure, application programming
    interface (API), graphical tools and online reports. With over 80K sample aliquots
    from 11,000+ cancer patients, spanning 38 unique disease cohorts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1
  tags: Metadata
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metadata/master/_listings/fire-browse-beta-api/openapi.md
x-common:
- type: x-website
  url: http://firebrowse.org
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---