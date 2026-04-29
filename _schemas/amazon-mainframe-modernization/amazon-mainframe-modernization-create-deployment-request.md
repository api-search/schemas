---
description: CreateDeploymentRequest schema from AWS Mainframe Modernization API
layout: schema
name: CreateDeploymentRequest
properties_list:
- description: ''
  name: applicationVersion
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: environmentId
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-create-deployment-request-schema.json
slug: amazon-mainframe-modernization-create-deployment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-deployment-request-schema.json\",\n  \"title\": \"CreateDeploymentRequest\",\n  \"description\": \"CreateDeploymentRequest schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the application to deploy.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier you provide to ensure the idempotency of the request to create a deployment. The service generates the clientToken\
  \ when the API call is triggered. The token expires after one hour, so if you retry the API within this timeframe with the same clientToken, you will get the same response. The service also handles deleting the clientToken after it expires. \"\n        }\n      ]\n    },\n    \"environmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The identifier of the runtime environment where you want to deploy this application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationVersion\",\n    \"environmentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-deployment-request-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: CreateDeploymentRequest
---
