---
description: Information about a scan.
layout: schema
name: ScanSummary
properties_list:
- description: ''
  name: createdAt
  type: object
- description: ''
  name: runId
  type: object
- description: ''
  name: scanName
  type: object
- description: ''
  name: scanNameArn
  type: object
- description: ''
  name: scanState
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-scan-summary-schema.json
slug: amazon-codeguru-security-scan-summary
source_filename: amazon-codeguru-security-scan-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-scan-summary-schema.json\",\n  \"title\": \"ScanSummary\",\n  \"description\": \"Information about a scan. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The time when the scan was created. \"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"The identifier for the scan run. \"\n        }\n      ]\n    },\n    \"scanName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanName\"\n        },\n        {\n          \"description\": \"The name of the\
  \ scan. \"\n        }\n      ]\n    },\n    \"scanNameArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanNameArn\"\n        },\n        {\n          \"description\": \"The ARN for the scan name.\"\n        }\n      ]\n    },\n    \"scanState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanState\"\n        },\n        {\n          \"description\": \"The state of the scan. A scan can be <code>In Progress</code>, <code>Complete</code>, or <code>Failed</code>. \"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the scan was last updated. A scan is updated when it is re-run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"createdAt\",\n    \"runId\",\n    \"scanName\",\n    \"scanState\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-scan-summary-schema.json
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: ScanSummary
---
