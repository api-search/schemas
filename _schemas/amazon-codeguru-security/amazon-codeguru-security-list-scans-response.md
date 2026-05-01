---
description: ListScansResponse schema from Amazon CodeGuru Security
layout: schema
name: ListScansResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: summaries
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-list-scans-response-schema.json
slug: amazon-codeguru-security-list-scans-response
source_filename: amazon-codeguru-security-list-scans-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-list-scans-response-schema.json\",\n  \"title\": \"ListScansResponse\",\n  \"description\": \"ListScansResponse schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token. You can use this in future calls to <code>ListScans</code> to continue listing results after the current page.\"\n        }\n      ]\n    },\n    \"summaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanSummaries\"\n        },\n        {\n          \"description\": \"A list of <code>ScanSummary</code> objects with information about all scans in an account.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-list-scans-response-schema.json
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: ListScansResponse
---
