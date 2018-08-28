swagger: "2.0"
x-collection-name: Click Meter
x-complete: 1
info:
  title: Click Meter
  description: api-dashboard-for-clickmeter-api
  contact:
    name: Api Support
    url: http://www.clickmeter.com/api
    email: api@clickmeter.com
  version: v2
host: apiv2.clickmeter.com:80
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/guests/{guestId}/{type}/permissions/patch:
    post:
      summary: Change the permission on a shared object
      description: Change the permission on a shared object.
      operationId: postAccountGuestsGuestTypePermissionsPatch
      x-api-path-slug: accountguestsguestidtypepermissionspatch-post
      parameters:
      - in: body
        name: body
        description: The patch permission request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: guestId
        description: Id of the guest
      - in: path
        name: type
        description: Can be datapoint or group
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
      - Type
      - Permissions
      - Patch
    put:
      summary: Change the permission on a shared object
      description: Change the permission on a shared object.
      operationId: putAccountGuestsGuestTypePermissionsPatch
      x-api-path-slug: accountguestsguestidtypepermissionspatch-put
      parameters:
      - in: body
        name: body
        description: The patch permission request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: guestId
        description: Id of the guest
      - in: path
        name: type
        description: Can be datapoint or group
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
      - Type
      - Permissions
      - Patch
  /conversions/{conversionId}/datapoints/batch/patch:
    put:
      summary: Modify the association between a conversion and multiple datapoints
      description: Modify the association between a conversion and multiple datapoints.
      operationId: putConversionsConversionDatapointsBatchPatch
      x-api-path-slug: conversionsconversioniddatapointsbatchpatch-put
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: body
        name: data
        description: Patch requests
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Datapoints
      - Batch
      - Patch
  /conversions/{conversionId}/datapoints/patch:
    put:
      summary: Modify the association between a conversion and a datapoint
      description: Modify the association between a conversion and a datapoint.
      operationId: putConversionsConversionDatapointsPatch
      x-api-path-slug: conversionsconversioniddatapointspatch-put
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: body
        name: data
        description: Patch request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Datapoints
      - Patch
  /tags/{tagId}/datapoints/patch:
    put:
      summary: Associate/Deassociate a tag with a datapoint
      description: Associate/deassociate a tag with a datapoint.
      operationId: putTagsTagDatapointsPatch
      x-api-path-slug: tagstagiddatapointspatch-put
      parameters:
      - in: body
        name: data
        description: The body patch
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tagId
        description: Id of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Datapoints
      - Patch
  /tags/{tagId}/groups/patch:
    put:
      summary: Associate/Deassociate a tag with a group
      description: Associate/deassociate a tag with a group.
      operationId: putTagsTagGroupsPatch
      x-api-path-slug: tagstagidgroupspatch-put
      parameters:
      - in: body
        name: data
        description: The body patch
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tagId
        description: Id of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Groups
      - Patch