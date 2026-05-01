---
description: MapFilterList schema
layout: schema
name: MapFilterList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-map-filter-list-schema.json
slug: inspector-map-filter-list
source_filename: inspector-map-filter-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-map-filter-list-schema.json\",\n  \"title\": \"MapFilterList\",\n  \"description\": \"MapFilterList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"comparison\",\n      \"key\"\n    ],\n    \"properties\": {\n      \"comparison\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/MapComparison\"\n          },\n          {\n            \"description\": \"The operator to use when comparing values in the filter.\"\n          }\n        ]\n      },\n      \"key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/MapKey\"\n          },\n          {\n            \"description\": \"The tag key used in the filter.\"\n          }\n        ]\n      },\n      \"value\": {\n    \
  \    \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/MapValue\"\n          },\n          {\n            \"description\": \"The tag value used in the filter.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that describes details of a map filter.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-map-filter-list-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: MapFilterList
---
