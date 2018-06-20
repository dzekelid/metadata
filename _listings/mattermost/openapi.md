---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-4-0-release--api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v5-0--details-heretagapiv3deprecation--looking-for-the-api-v3-reference-it-has-moved-herehttpsapi-mattermost-comv3-
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{file_id}/info:
    get:
      summary: Get metadata for a file
      description: |-
        Gets a file's info.
        ##### Permissions
        Must have `read_channel` permission or be uploader of the file.
      operationId: gets-a-files-info-permissionsmust-have-read-channel-permission-or-be-uploader-of-the-file
      x-api-path-slug: filesfile-idinfo-get
      parameters:
      - in: path
        name: file_id
        description: The ID of the file info to get
      responses:
        200:
          description: OK
      tags:
      - Metadataa
      - File
  /saml/metadata:
    get:
      summary: Get metadata
      description: |-
        Get SAML metadata from the server. SAML must be configured properly.
        ##### Permissions
        No permission required.
      operationId: get-saml-metadata-from-the-server-saml-must-be-configured-properly-permissionsno-permission-required
      x-api-path-slug: samlmetadata-get
      responses:
        200:
          description: OK
      tags:
      - Metadata
---