---
description: Contains information about the error that caused a finding to fail to be retrieved.
layout: schema
name: BatchGetFindingsError
properties_list:
- description: ''
  name: errorCode
  type: object
- description: ''
  name: findingId
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: scanName
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-batch-get-findings-error-schema.json
slug: amazon-codeguru-security-batch-get-findings-error
source_filename: amazon-codeguru-security-batch-get-findings-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-batch-get-findings-error-schema.json\",\n  \"title\": \"BatchGetFindingsError\",\n  \"description\": \"Contains information about the error that caused a finding to fail to be retrieved.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorCode\"\n        },\n        {\n          \"description\": \"A code associated with the type of error.\"\n        }\n      ]\n    },\n    \"findingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The finding ID of the finding that was not fetched.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Describes the error.\"\n        }\n      ]\n    },\n    \"scanName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanName\"\n        },\n        {\n          \"description\": \"The name of the scan that generated the finding.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errorCode\",\n    \"findingId\",\n    \"message\",\n    \"scanName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-batch-get-findings-error-schema.json
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: BatchGetFindingsError
---
