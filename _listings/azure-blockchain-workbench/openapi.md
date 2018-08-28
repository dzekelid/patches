swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 1
info:
  title: Azure Blockchain Workbench REST API
  description: the-azure-blockchain-workbench-rest-api-is-a-workbench-extensibility-point-which-allows-developers-to-create-and-manage-blockchain-applications-manage-users-and-organizations-within-a-consortium-integrate-blockchain-applications-into-services-and-platforms-perform-transactions-on-a-blockchain-and-retrieve-transactional-and-contract-data-from-a-blockchain-
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