{
  "info": {
    "name": "Pay Run.IO Patches the DPS message",
    "_postman_id": "8112abbe-d473-4c64-bf4e-46c7abec0a83",
    "description": "Patches the specified DPS message with the supplied values",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "DPMessage",
      "item": [
        {
          "id": "106ba96b-a3cc-4822-9bd5-992e4f448f66",
          "name": "GetDpsMessageFromEmployer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/DpsMessage/:DpsMessageId"
              ],
              "variable": [
                {
                  "id": "DpsMessageId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the DPS message"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46783634-a2ca-4f9d-a9bb-e24645f3b0d6"
            }
          ]
        },
        {
          "id": "9e981c31-5528-41c1-bf8c-44ec139baf4b",
          "name": "DeleteDpsMessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/DpsMessage/:DpsMessageId"
              ],
              "variable": [
                {
                  "id": "DpsMessageId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the DPS message"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07178969-8aa2-4113-964e-0274e319a57e"
            }
          ]
        }
      ]
    },
    {
      "name": "Patches",
      "item": [
        {
          "id": "0f2dfa5d-c9e0-4a2a-80ec-eff0bd5f67a0",
          "name": "PatchDpsMessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/DpsMessage/:DpsMessageId"
              ],
              "variable": [
                {
                  "id": "DpsMessageId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Patches the specified DPS message with the supplied values"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca484b51-f3d3-4d58-a27b-56ec34824055"
            }
          ]
        }
      ]
    }
  ]
}