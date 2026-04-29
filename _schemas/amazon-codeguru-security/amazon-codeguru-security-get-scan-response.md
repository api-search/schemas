---
description: GetScanResponse schema from Amazon CodeGuru Security
layout: schema
name: GetScanResponse
properties_list:
- description: ''
  name: analysisType
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: numberOfRevisions
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
schema_file: json-schema/amazon-codeguru-security-get-scan-response-schema.json
slug: amazon-codeguru-security-get-scan-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-get-scan-response-schema.json\",\n  \"title\": \"GetScanResponse\",\n  \"description\": \"GetScanResponse schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analysisType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalysisType\"\n        },\n        {\n          \"description\": \"The type of analysis CodeGuru Security performed in the scan, either <code>Security</code> or <code>All</code>. The <code>Security</code> type only generates findings related to security. The <code>All</code> type generates both security findings and quality findings.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n\
  \        {\n          \"description\": \"The time the scan was created.\"\n        }\n      ]\n    },\n    \"numberOfRevisions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of times a scan has been re-run on a revised resource.\"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID that identifies the individual scan run.\"\n        }\n      ]\n    },\n    \"scanName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanName\"\n        },\n        {\n          \"description\": \"The name of the scan.\"\n        }\n      ]\n    },\n    \"scanNameArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanNameArn\"\n        },\n        {\n          \"description\": \"The ARN for the scan name.\"\n\
  \        }\n      ]\n    },\n    \"scanState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanState\"\n        },\n        {\n          \"description\": \"The current state of the scan. Pass either <code>InProgress</code>, <code>Successful</code>, or <code>Failed</code>.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the scan was last updated. Only available for <code>STANDARD</code> scan types.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"analysisType\",\n    \"createdAt\",\n    \"runId\",\n    \"scanName\",\n    \"scanState\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-get-scan-response-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: GetScanResponse
---
