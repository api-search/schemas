---
description: DeleteFilterRequest schema
layout: schema
name: DeleteFilterRequest
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-delete-filter-request-schema.json
slug: inspector-delete-filter-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-delete-filter-request-schema.json\",\n  \"title\": \"DeleteFilterRequest\",\n  \"description\": \"DeleteFilterRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the filter to be deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-delete-filter-request-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: DeleteFilterRequest
---
