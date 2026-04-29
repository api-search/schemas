---
description: CreateScanResponse schema from Amazon CodeGuru Security
layout: schema
name: CreateScanResponse
properties_list:
- description: ''
  name: resourceId
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
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-create-scan-response-schema.json
slug: amazon-codeguru-security-create-scan-response
source_filename: amazon-codeguru-security-create-scan-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-create-scan-response-schema.json\",\n  \"title\": \"CreateScanResponse\",\n  \"description\": \"CreateScanResponse schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for the resource object that contains resources that were scanned.\"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID that identifies the individual scan run.\"\n        }\n      ]\n    },\n    \"scanName\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/ScanName\"\n        },\n        {\n          \"description\": \"The name of the scan.\"\n        }\n      ]\n    },\n    \"scanNameArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanNameArn\"\n        },\n        {\n          \"description\": \"The ARN for the scan name.\"\n        }\n      ]\n    },\n    \"scanState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanState\"\n        },\n        {\n          \"description\": \"The current state of the scan. Returns either <code>InProgress</code>, <code>Successful</code>, or <code>Failed</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceId\",\n    \"runId\",\n    \"scanName\",\n    \"scanState\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-create-scan-response-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: CreateScanResponse
---
