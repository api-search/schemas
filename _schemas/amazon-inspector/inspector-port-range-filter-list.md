---
description: PortRangeFilterList schema
layout: schema
name: PortRangeFilterList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-port-range-filter-list-schema.json
slug: inspector-port-range-filter-list
source_filename: inspector-port-range-filter-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-port-range-filter-list-schema.json\",\n  \"title\": \"PortRangeFilterList\",\n  \"description\": \"PortRangeFilterList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"beginInclusive\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Port\"\n          },\n          {\n            \"description\": \"The port number the port range begins at.\"\n          }\n        ]\n      },\n      \"endInclusive\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Port\"\n          },\n          {\n            \"description\": \"The port number the port range ends at.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that describes the details of a port range\
  \ filter.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-port-range-filter-list-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: PortRangeFilterList
---
