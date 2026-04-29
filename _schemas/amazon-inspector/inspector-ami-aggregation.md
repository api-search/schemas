---
description: The details that define an aggregation based on Amazon machine images (AMIs).
layout: schema
name: AmiAggregation
properties_list:
- description: ''
  name: amis
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-ami-aggregation-schema.json
slug: inspector-ami-aggregation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-ami-aggregation-schema.json\",\n  \"title\": \"AmiAggregation\",\n  \"description\": \"The details that define an aggregation based on Amazon machine images (AMIs).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The IDs of AMIs to aggregate findings for.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmiSortBy\"\n        },\n        {\n          \"description\": \"The value to sort results by.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n\
  \          \"description\": \"The order to sort results by.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-ami-aggregation-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AmiAggregation
---
