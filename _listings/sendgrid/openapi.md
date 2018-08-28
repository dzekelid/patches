swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts/{alert_id}:
    patch:
      summary: Patch Alerts Alert
      description: "**This endpoint allows you to update an alert.**\n\nAlerts allow
        you to specify an email address to receive notifications regarding your email
        usage or statistics. \n* Usage alerts allow you to set the threshold at which
        an alert will be sent.\n* Stats notifications allow you to set how frequently
        you would like to receive email statistics reports. For example, \"daily\",
        \"weekly\", or \"monthly\".\n\nFor more information about alerts, please see
        our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
      operationId: alerts.alert_id.patch
      x-api-path-slug: alertsalert-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Alerts
      - Alert
  /api_keys/{api_key_id}:
    patch:
      summary: Patch Api Keys Api Key
      description: |-
        **This endpoint allows you to update the name of an existing API Key.**

        A JSON request body with a "name" property is required.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

        ## URI Parameters

        | URI Parameter   | Type  | Required?  | Description  |
        |---|---|---|---|
        |api_key_id |string | required | The ID of the API Key you are updating.|
      operationId: api_keys.api_key_id.patch
      x-api-path-slug: api-keysapi-key-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
      - Api
      - Key