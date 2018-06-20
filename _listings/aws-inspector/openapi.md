---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 1
info:
  title: AWS Inspector API
  version: 1.0.0
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
---