---
description: BatchGetFindingDetailsResponse schema
layout: schema
name: BatchGetFindingDetailsResponse
properties_list:
- description: ''
  name: errors
  type: object
- description: ''
  name: findingDetails
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-finding-details-response-schema.json
slug: inspector-batch-get-finding-details-response
source_filename: inspector-batch-get-finding-details-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-finding-details-response-schema.json\",\n  \"title\": \"BatchGetFindingDetailsResponse\",\n  \"description\": \"BatchGetFindingDetailsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingDetailsErrorList\"\n        },\n        {\n          \"description\": \"Error information for findings that details could not be returned for.\"\n        }\n      ]\n    },\n    \"findingDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingDetails\"\n        },\n        {\n          \"description\": \"A finding's vulnerability details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-finding-details-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetFindingDetailsResponse
---
