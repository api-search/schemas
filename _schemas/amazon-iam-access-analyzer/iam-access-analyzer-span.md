---
description: A span in a policy. The span consists of a start position (inclusive) and end position (exclusive).
layout: schema
name: Span
properties_list:
- description: ''
  name: start
  type: object
- description: ''
  name: end
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-span-schema.json
slug: iam-access-analyzer-span
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-span-schema.json\",\n  \"title\": \"Span\",\n  \"description\": \"A span in a policy. The span consists of a start position (inclusive) and end position (exclusive).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Position\"\n        },\n        {\n          \"description\": \"The start position of the span (inclusive).\"\n        }\n      ]\n    },\n    \"end\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Position\"\n        },\n        {\n          \"description\": \"The end position of the span (exclusive).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"start\",\n    \"end\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-span-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: Span
---
