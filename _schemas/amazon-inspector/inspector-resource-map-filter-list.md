---
description: ResourceMapFilterList schema
layout: schema
name: ResourceMapFilterList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-resource-map-filter-list-schema.json
slug: inspector-resource-map-filter-list
source_filename: inspector-resource-map-filter-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-map-filter-list-schema.json\",\n  \"title\": \"ResourceMapFilterList\",\n  \"description\": \"ResourceMapFilterList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"comparison\",\n      \"key\"\n    ],\n    \"properties\": {\n      \"comparison\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceMapComparison\"\n          },\n          {\n            \"description\": \"The filter's comparison.\"\n          }\n        ]\n      },\n      \"key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The filter's key.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"\
  allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The filter's value.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A resource map filter for a software bill of material report.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-map-filter-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ResourceMapFilterList
---
