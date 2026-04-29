---
description: EventList schema from ARGUS Enterprise API
layout: schema
name: EventList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: pagination
  type: object
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-event-list-schema.json
slug: argus-enterprise-event-list
source_filename: argus-enterprise-event-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-event-list-schema.json\",\n  \"title\": \"EventList\",\n  \"description\": \"EventList schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Event\"\n      }\n    },\n    \"pagination\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"page\": {\n          \"type\": \"integer\"\n        },\n        \"pageSize\": {\n          \"type\": \"integer\"\n        },\n        \"totalItems\": {\n          \"type\": \"integer\"\n        },\n        \"totalPages\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-event-list-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: EventList
---
