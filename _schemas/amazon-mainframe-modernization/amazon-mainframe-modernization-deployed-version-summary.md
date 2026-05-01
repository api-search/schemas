---
description: Contains a summary of a deployed application.
layout: schema
name: DeployedVersionSummary
properties_list:
- description: ''
  name: applicationVersion
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-deployed-version-summary-schema.json
slug: amazon-mainframe-modernization-deployed-version-summary
source_filename: amazon-mainframe-modernization-deployed-version-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-deployed-version-summary-schema.json\",\n  \"title\": \"DeployedVersionSummary\",\n  \"description\": \"Contains a summary of a deployed application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the deployed application.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentLifecycle\"\n        },\n        {\n          \"description\": \"The status of the deployment.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The reason for the reported status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationVersion\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-deployed-version-summary-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: DeployedVersionSummary
---
