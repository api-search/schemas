---
description: WorkOrderList schema from 1Factory API
layout: schema
name: WorkOrderList
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-work-order-list-schema.json
slug: 1factory-work-order-list
source_filename: 1factory-work-order-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-work-order-list-schema.json\",\n  \"title\": \"WorkOrderList\",\n  \"description\": \"WorkOrderList schema from 1Factory API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"insp_ident_1\"\n    ],\n    \"properties\": {\n      \"insp_ident_1\": {\n        \"$ref\": \"#/components/schemas/insp_ident_1\"\n      },\n      \"insp_ident_2\": {\n        \"$ref\": \"#/components/schemas/insp_ident_2\"\n      },\n      \"lot_size\": {\n        \"type\": \"integer\",\n        \"format\": \"int32\",\n        \"nullable\": true,\n        \"minimum\": 0,\n        \"description\": \"The lot size for this order. (Optional).\",\n        \"example\": 50\n      }\n    }\n  },\n  \"minItems\": 0,\n  \"maxItems\": 5000\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-work-order-list-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: WorkOrderList
---
