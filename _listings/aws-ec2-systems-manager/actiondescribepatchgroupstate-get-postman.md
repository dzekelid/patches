{
  "info": {
    "name": "Amazon EC2 Systems Manager API Describe Patch Group State",
    "_postman_id": "74e9f626-2825-43da-9f9f-b0e3947832c8",
    "description": "Returns high-level aggregated patch compliance state for a patch group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Instance",
      "item": [
        {
          "id": "21c02e56-9892-49d6-9c7a-a8e30a8b33e5",
          "name": "describeInstancePatchStates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStates?InstanceIds=InstanceIds&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state of one or more instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4887dc77-f5ef-41ba-84e6-5c2b9d564083"
            }
          ]
        },
        {
          "id": "bd1ec44d-f005-469d-8e5f-1bb5fffd3267",
          "name": "describeInstancePatchStatesForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStatesForPatchGroup?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state for the instances in the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3fc373b-6e25-44e4-9152-bf1135ae1246"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "45e1c8fd-4928-4dc5-9a3e-07c476f0d925",
          "name": "describePatchGroupState",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroupState?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns high-level aggregated patch compliance state for a patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "873589cc-4470-43b5-b735-61bee81fcd54"
            }
          ]
        }
      ]
    }
  ]
}