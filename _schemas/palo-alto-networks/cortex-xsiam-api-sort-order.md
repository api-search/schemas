---
description: Sorting specification for result sets.
layout: schema
name: SortOrder
properties_list:
- description: ''
  name: field
  type: string
- description: ''
  name: keyword
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsiam-api-sort-order-schema.json
slug: cortex-xsiam-api-sort-order
source_filename: cortex-xsiam-api-sort-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SortOrder\",\n  \"description\": \"Sorting specification for result sets.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-api-sort-order-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"type\": \"string\"\n    },\n    \"keyword\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"asc\",\n        \"desc\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-api-sort-order-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SortOrder
---
