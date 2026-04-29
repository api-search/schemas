---
description: A filter criterion for querying Xpanse resources.
layout: schema
name: Filter
properties_list:
- description: Field name to filter on.
  name: field
  type: string
- description: ''
  name: operator
  type: string
- description: Filter value (string, integer, or array for "in" operator).
  name: value
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xpanse-api-filter-schema.json
slug: cortex-xpanse-api-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Filter\",\n  \"description\": \"A filter criterion for querying Xpanse resources.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-filter-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"type\": \"string\",\n      \"description\": \"Field name to filter on.\"\n    },\n    \"operator\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"in\",\n        \"contains\",\n        \"gte\",\n        \"lte\",\n        \"eq\",\n        \"neq\"\n      ]\n    },\n    \"value\": {\n      \"description\": \"Filter value (string, integer, or array for \\\"in\\\" operator).\",\n      \"oneOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n      \
  \      \"oneOf\": [\n              {\n                \"type\": \"string\"\n              },\n              {\n                \"type\": \"integer\"\n              }\n            ]\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"field\",\n    \"operator\",\n    \"value\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-filter-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Filter
---
