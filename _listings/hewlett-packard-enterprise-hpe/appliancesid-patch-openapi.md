---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Patch Appliances
  description: Update properties of an appliance.
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /appliances/{id}:
    patch:
      summary: Patch Appliances
      description: Update properties of an appliance.
      operationId: UpdateAppliance
      x-api-path-slug: appliancesid-patch
      parameters:
      - in: body
        name: body
        description: List of appliance updates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of appliance to update
      responses:
        200:
          description: OK
      tags:
      - Appliances
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