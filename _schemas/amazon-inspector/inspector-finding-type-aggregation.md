---
description: The details that define an aggregation based on finding type.
layout: schema
name: FindingTypeAggregation
properties_list:
- description: ''
  name: findingType
  type: object
- description: ''
  name: resourceType
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-finding-type-aggregation-schema.json
slug: inspector-finding-type-aggregation
source_filename: inspector-finding-type-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-finding-type-aggregation-schema.json\",\n  \"title\": \"FindingTypeAggregation\",\n  \"description\": \"The details that define an aggregation based on finding type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationFindingType\"\n        },\n        {\n          \"description\": \"The finding type to aggregate.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationResourceType\"\n        },\n        {\n          \"description\": \"The resource type to aggregate.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingTypeSortBy\"\
  \n        },\n        {\n          \"description\": \"The value to sort results by.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"The order to sort results by.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-finding-type-aggregation-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: FindingTypeAggregation
---
