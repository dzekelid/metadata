---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 0
info:
  title: AWS Inspector API Get Telemetry Metadata
  version: 1.0.0
  description: |-
    Information about the data that is collected for the specified assessment
             run.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetTelemetryMetadata:
    get:
      summary: Get Telemetry Metadata
      description: |-
        Information about the data that is collected for the specified assessment
                 run.
      operationId: getTelemetryMetadata
      x-api-path-slug: actiongettelemetrymetadata-get
      parameters:
      - in: query
        name: assessmentRunArn
        description: The ARN that specifies the assessment run that has the telemetry
          data that you want         to obtain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Telemetry Metadata
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