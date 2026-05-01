---
description: ResourceStringFilterList schema
layout: schema
name: ResourceStringFilterList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-resource-string-filter-list-schema.json
slug: inspector-resource-string-filter-list
source_filename: inspector-resource-string-filter-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-string-filter-list-schema.json\",\n  \"title\": \"ResourceStringFilterList\",\n  \"description\": \"ResourceStringFilterList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"comparison\",\n      \"value\"\n    ],\n    \"properties\": {\n      \"comparison\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceStringComparison\"\n          },\n          {\n            \"description\": \"The filter's comparison.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceStringInput\"\n          },\n          {\n            \"description\": \"The filter's value.\"\n          }\n        ]\n      }\n    },\n\
  \    \"description\": \"A resource string filter for a software bill of materials report.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-string-filter-list-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ResourceStringFilterList
---
