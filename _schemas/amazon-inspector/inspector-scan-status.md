---
description: The status of the scan.
layout: schema
name: ScanStatus
properties_list:
- description: ''
  name: reason
  type: object
- description: ''
  name: statusCode
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-scan-status-schema.json
slug: inspector-scan-status
source_filename: inspector-scan-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-scan-status-schema.json\",\n  \"title\": \"ScanStatus\",\n  \"description\": \"The status of the scan.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanStatusReason\"\n        },\n        {\n          \"description\": \"The reason for the scan.\"\n        }\n      ]\n    },\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanStatusCode\"\n        },\n        {\n          \"description\": \"The status code of the scan.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"reason\",\n    \"statusCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-scan-status-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ScanStatus
---
