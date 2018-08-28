---
swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 0
info:
  title: Azure Blockchain Workbench Patch Applications Enable
  description: |-
    Enables the specified blockchain application. This method can only be performed by users who are
                 Workbench administrators.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/applications/{applicationId}/disable:
    patch:
      summary: Patch Applications Disable
      description: |-
        Disables the specified blockchain application. This method can only be performed by users who are
                     Workbench administrators.
      operationId: ApplicationDisable
      x-api-path-slug: apiv1applicationsapplicationiddisable-patch
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Disable
  /api/v1/applications/{applicationId}/enable:
    patch:
      summary: Patch Applications Enable
      description: |-
        Enables the specified blockchain application. This method can only be performed by users who are
                     Workbench administrators.
      operationId: ApplicationEnable
      x-api-path-slug: apiv1applicationsapplicationidenable-patch
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Enable
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