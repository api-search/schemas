---
description: A virtual tag configuration used for resource allocation and filtering in Finout, enabling cost attribution to teams, services, environments, and customers even when native tagging is incomplete.
layout: schema
name: Finout Virtual Tag
properties_list:
- description: The unique identifier of the virtual tag.
  name: id
  type: string
- description: The unique identifier of the account associated with the virtual tag.
  name: accountId
  type: string
- description: The name of the virtual tag.
  name: name
  type: string
- description: An array of rule objects that define the filtering criteria for the virtual tag.
  name: rules
  type: array
provider_name: Finout
provider_slug: finout
schema_file: json-schema/virtual-tag.json
slug: virtual-tag
source_filename: virtual-tag.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/finout/blob/main/json-schema/virtual-tag.json\",\n  \"title\": \"Finout Virtual Tag\",\n  \"description\": \"A virtual tag configuration used for resource allocation and filtering in Finout, enabling cost attribution to teams, services, environments, and customers even when native tagging is incomplete.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the virtual tag.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the account associated with the virtual tag.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the virtual tag.\"\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"An array of rule objects that define the filtering criteria\
  \ for the virtual tag.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name or value assigned when the rule matches.\"\n          },\n          \"filter\": {\n            \"$ref\": \"https://github.com/api-evangelist/finout/blob/main/json-schema/virtual-tag.json#/$defs/FilterObject\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"$defs\": {\n    \"FilterObject\": {\n      \"type\": \"object\",\n      \"description\": \"A filter object used to narrow query results, supporting logical AND/OR grouping and various operators.\",\n      \"properties\": {\n        \"costCenter\": {\n          \"type\": \"string\",\n          \"description\": \"The cost center to filter on (e.g., AWS, GCP, Azure).\"\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The MegaBill key to filter by.\"\n \
  \       },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name for the filter field.\"\n        },\n        \"operator\": {\n          \"type\": \"string\",\n          \"description\": \"The filter operator.\",\n          \"enum\": [\"oneOf\", \"notOneOf\", \"is\", \"isNot\", \"contains\", \"notContains\", \"exists\", \"notExists\"]\n        },\n        \"value\": {\n          \"description\": \"The value or values to match against.\",\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n          ]\n        },\n        \"and\": {\n          \"type\": \"array\",\n          \"description\": \"Logical AND grouping of filter conditions.\",\n          \"items\": {\n            \"$ref\": \"https://github.com/api-evangelist/finout/blob/main/json-schema/virtual-tag.json#/$defs/FilterObject\"\n          }\n        },\n        \"or\": {\n          \"type\"\
  : \"array\",\n          \"description\": \"Logical OR grouping of filter conditions.\",\n          \"items\": {\n            \"$ref\": \"https://github.com/api-evangelist/finout/blob/main/json-schema/virtual-tag.json#/$defs/FilterObject\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/finout/refs/heads/main/json-schema/virtual-tag.json
tags:
- Budgets
- Costs
- FinOps
title: Finout Virtual Tag
---
