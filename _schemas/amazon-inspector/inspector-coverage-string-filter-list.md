---
description: CoverageStringFilterList schema
layout: schema
name: CoverageStringFilterList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-coverage-string-filter-list-schema.json
slug: inspector-coverage-string-filter-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-coverage-string-filter-list-schema.json\",\n  \"title\": \"CoverageStringFilterList\",\n  \"description\": \"CoverageStringFilterList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"comparison\",\n      \"value\"\n    ],\n    \"properties\": {\n      \"comparison\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CoverageStringComparison\"\n          },\n          {\n            \"description\": \"The operator to compare strings on.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CoverageStringInput\"\n          },\n          {\n            \"description\": \"The value to compare strings on.\"\n          }\n   \
  \     ]\n      }\n    },\n    \"description\": \"Contains details of a coverage string filter.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-coverage-string-filter-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CoverageStringFilterList
---
