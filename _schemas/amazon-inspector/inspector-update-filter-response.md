---
description: UpdateFilterResponse schema
layout: schema
name: UpdateFilterResponse
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-update-filter-response-schema.json
slug: inspector-update-filter-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-update-filter-response-schema.json\",\n  \"title\": \"UpdateFilterResponse\",\n  \"description\": \"UpdateFilterResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the successfully updated filter.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-update-filter-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: UpdateFilterResponse
---
