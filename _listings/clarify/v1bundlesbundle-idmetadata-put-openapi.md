---
swagger: "2.0"
x-collection-name: Clarify
x-complete: 0
info:
  title: Clarify Update bundle metadata
  description: Update the metadata for a bundle.The metadata is a single-level JSON
    object of your own definition, containing key-values that can be searched and
    filtered on. Metadata can be used to hold text such as names, titles, descriptions
    and values for segregating bundles, for example by user, topic, folder name etc.
    The keys (property names) can be up to 64 characters and must contain only alphanumeric
    characters and underscore (but not start with underscore) and must not be a reserved
    name. Reserved names are &quot;true&quot;, &quot;false&quot;, and &quot;null&quot;.
    Values can be strings, numbers, boolean true/false, date-times represented as
    a string in ISO 8601 format (ex. &quot;2014-02-25T14:23:45.000Z&quot;), or an
    array of these primitive types. Strings can be up to 2000 characters and strings
    in arrays can be up to 128 characters each. Nested objects are not allowed. Metadata
    can contain up to 50 key-value pairs up to a total JSON size of 4000 characters.To
    clear the metadata for a bundle, send data={}.If version specified, the metadata
    will only be updated if the current version matches this parameter value. If the
    version doesn't match, a 409 Conflict will be returned. If version not specified,
    the metadata will always be updated.
  version: 1.3.4
host: api.clarify.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/bundles/{bundle_id}/metadata:
    delete:
      summary: Delete bundle metadata
      description: Delete the metadata of a bundle and set data to {} (empty object.)
        This is functionally equivalent to an update metadata request with data set
        to {}.Successful response will be a HTTP code 204 with an empty body.
      operationId: deleteV1BundlesBundleMetadata
      x-api-path-slug: v1bundlesbundle-idmetadata-delete
      parameters:
      - in: path
        name: bundle_id
        description: id of a bundle
      responses:
        200:
          description: OK
      tags:
      - Bundle
      - Metadata
    get:
      summary: Get bundle metadata
      description: Gets the metadata for a bundle.
      operationId: getV1BundlesBundleMetadata
      x-api-path-slug: v1bundlesbundle-idmetadata-get
      parameters:
      - in: path
        name: bundle_id
        description: id of a bundle
      responses:
        200:
          description: OK
      tags:
      - Bundle
      - Metadata
    put:
      summary: Update bundle metadata
      description: Update the metadata for a bundle.The metadata is a single-level
        JSON object of your own definition, containing key-values that can be searched
        and filtered on. Metadata can be used to hold text such as names, titles,
        descriptions and values for segregating bundles, for example by user, topic,
        folder name etc. The keys (property names) can be up to 64 characters and
        must contain only alphanumeric characters and underscore (but not start with
        underscore) and must not be a reserved name. Reserved names are &quot;true&quot;,
        &quot;false&quot;, and &quot;null&quot;. Values can be strings, numbers, boolean
        true/false, date-times represented as a string in ISO 8601 format (ex. &quot;2014-02-25T14:23:45.000Z&quot;),
        or an array of these primitive types. Strings can be up to 2000 characters
        and strings in arrays can be up to 128 characters each. Nested objects are
        not allowed. Metadata can contain up to 50 key-value pairs up to a total JSON
        size of 4000 characters.To clear the metadata for a bundle, send data={}.If
        version specified, the metadata will only be updated if the current version
        matches this parameter value. If the version doesn't match, a 409 Conflict
        will be returned. If version not specified, the metadata will always be updated.
      operationId: putV1BundlesBundleMetadata
      x-api-path-slug: v1bundlesbundle-idmetadata-put
      parameters:
      - in: path
        name: bundle_id
        description: id of a bundle
      - in: formData
        name: data
        description: User-defined JSON data associated with the bundle
      - in: formData
        name: version
        description: Object version
      responses:
        200:
          description: OK
      tags:
      - Bundle
      - Metadata
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