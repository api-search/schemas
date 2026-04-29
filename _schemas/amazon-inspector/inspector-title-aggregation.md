---
description: The details that define an aggregation based on finding title.
layout: schema
name: TitleAggregation
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
- description: ''
  name: titles
  type: object
- description: ''
  name: vulnerabilityIds
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-title-aggregation-schema.json
slug: inspector-title-aggregation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-title-aggregation-schema.json\",\n  \"title\": \"TitleAggregation\",\n  \"description\": \"The details that define an aggregation based on finding title.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationFindingType\"\n        },\n        {\n          \"description\": \"The type of finding to aggregate on.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationResourceType\"\n        },\n        {\n          \"description\": \"The resource type to aggregate on.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TitleSortBy\"\n \
  \       },\n        {\n          \"description\": \"The value to sort results by.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"The order to sort results by.\"\n        }\n      ]\n    },\n    \"titles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The finding titles to aggregate on.\"\n        }\n      ]\n    },\n    \"vulnerabilityIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The vulnerability IDs of the findings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-title-aggregation-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: TitleAggregation
---
