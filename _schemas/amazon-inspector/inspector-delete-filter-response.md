---
description: DeleteFilterResponse schema
layout: schema
name: DeleteFilterResponse
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-delete-filter-response-schema.json
slug: inspector-delete-filter-response
source_filename: inspector-delete-filter-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-delete-filter-response-schema.json\",\n  \"title\": \"DeleteFilterResponse\",\n  \"description\": \"DeleteFilterResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the filter that has been deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-delete-filter-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: DeleteFilterResponse
---
