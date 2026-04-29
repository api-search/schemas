---
description: StringFilterList schema
layout: schema
name: StringFilterList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-string-filter-list-schema.json
slug: inspector-string-filter-list
source_filename: inspector-string-filter-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-string-filter-list-schema.json\",\n  \"title\": \"StringFilterList\",\n  \"description\": \"StringFilterList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"comparison\",\n      \"value\"\n    ],\n    \"properties\": {\n      \"comparison\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StringComparison\"\n          },\n          {\n            \"description\": \"The operator to use when comparing values in the filter.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StringInput\"\n          },\n          {\n            \"description\": \"The value to filter on.\"\n          }\n        ]\n      }\n    },\n    \"\
  description\": \"An object that describes the details of a string filter.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-string-filter-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: StringFilterList
---
