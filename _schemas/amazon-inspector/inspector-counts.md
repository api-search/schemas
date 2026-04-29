---
description: a structure that contains information on the count of resources within a group.
layout: schema
name: Counts
properties_list:
- description: ''
  name: count
  type: object
- description: ''
  name: groupKey
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-counts-schema.json
slug: inspector-counts
source_filename: inspector-counts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-counts-schema.json\",\n  \"title\": \"Counts\",\n  \"description\": \"a structure that contains information on the count of resources within a group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggCounts\"\n        },\n        {\n          \"description\": \"The number of resources.\"\n        }\n      ]\n    },\n    \"groupKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupKey\"\n        },\n        {\n          \"description\": \"The key associated with this group\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-counts-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: Counts
---
