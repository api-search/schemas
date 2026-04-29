---
description: NumberFilterList schema
layout: schema
name: NumberFilterList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-number-filter-list-schema.json
slug: inspector-number-filter-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-number-filter-list-schema.json\",\n  \"title\": \"NumberFilterList\",\n  \"description\": \"NumberFilterList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"lowerInclusive\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Double\"\n          },\n          {\n            \"description\": \"The lowest number to be included in the filter.\"\n          }\n        ]\n      },\n      \"upperInclusive\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Double\"\n          },\n          {\n            \"description\": \"The highest number to be included in the filter.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that describes the details\
  \ of a number filter.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-number-filter-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: NumberFilterList
---
