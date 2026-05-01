---
description: A subset of information about a specific deployment.
layout: schema
name: DeploymentSummary
properties_list:
- description: ''
  name: applicationId
  type: object
- description: ''
  name: applicationVersion
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: environmentId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-deployment-summary-schema.json
slug: amazon-mainframe-modernization-deployment-summary
source_filename: amazon-mainframe-modernization-deployment-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-deployment-summary-schema.json\",\n  \"title\": \"DeploymentSummary\",\n  \"description\": \"A subset of information about a specific deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the application.\"\n        }\n      ]\n    },\n    \"applicationVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the application.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The timestamp when the deployment was created.\"\n        }\n      ]\n    },\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the deployment.\"\n        }\n      ]\n    },\n    \"environmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the runtime environment.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentLifecycle\"\n        },\n        {\n          \"description\": \"The current status of the deployment.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\"\
  : \"The reason for the reported status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationId\",\n    \"applicationVersion\",\n    \"creationTime\",\n    \"deploymentId\",\n    \"environmentId\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-deployment-summary-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: DeploymentSummary
---
