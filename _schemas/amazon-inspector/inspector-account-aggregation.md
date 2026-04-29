---
description: An object that contains details about an aggregation response based on Amazon Web Services accounts.
layout: schema
name: AccountAggregation
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
schema_file: json-schema/inspector-account-aggregation-schema.json
slug: inspector-account-aggregation
source_filename: inspector-account-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-aggregation-schema.json\",\n  \"title\": \"AccountAggregation\",\n  \"description\": \"An object that contains details about an aggregation response based on Amazon Web Services accounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationFindingType\"\n        },\n        {\n          \"description\": \"The type of finding.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationResourceType\"\n        },\n        {\n          \"description\": \"The type of resource.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountSortBy\"\
  \n        },\n        {\n          \"description\": \"The value to sort by.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"The sort order (ascending or descending).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-aggregation-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AccountAggregation
---
