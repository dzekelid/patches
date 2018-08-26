---
swagger: "2.0"
x-collection-name: Azure DocumentDB
x-complete: 1
info:
  title: DocumentDB
  description: azure-documentdb-database-service-resource-provider-rest-api
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}:
    patch:
      summary: Database Accounts Patch
      description: Patches the properties of an existing Azure DocumentDB database
        account.
      operationId: DatabaseAccounts_Patch
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountname-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: updateParameters
        description: The tags parameter to patch for the current database account
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - Patch
---