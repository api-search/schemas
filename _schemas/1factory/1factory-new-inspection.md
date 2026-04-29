---
description: NewInspection schema from 1Factory API
layout: schema
name: NewInspection
properties_list:
- description: ''
  name: insp_ident_1
  type: object
- description: ''
  name: insp_ident_2
  type: object
- description: ''
  name: insp_ident_3
  type: object
- description: ''
  name: part_number
  type: object
- description: ''
  name: rev
  type: object
- description: ''
  name: inspection_type
  type: object
- description: ''
  name: lot_size
  type: object
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-new-inspection-schema.json
slug: 1factory-new-inspection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-new-inspection-schema.json\",\n  \"title\": \"NewInspection\",\n  \"description\": \"NewInspection schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"insp_ident_1\": {\n      \"$ref\": \"#/components/schemas/insp_ident_1\"\n    },\n    \"insp_ident_2\": {\n      \"$ref\": \"#/components/schemas/insp_ident_2\"\n    },\n    \"insp_ident_3\": {\n      \"$ref\": \"#/components/schemas/insp_ident_3\"\n    },\n    \"part_number\": {\n      \"$ref\": \"#/components/schemas/part_number\"\n    },\n    \"rev\": {\n      \"$ref\": \"#/components/schemas/rev\"\n    },\n    \"inspection_type\": {\n      \"$ref\": \"#/components/schemas/inspection_type\"\n    },\n    \"lot_size\": {\n      \"$ref\": \"#/components/schemas/lot_size\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-new-inspection-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: NewInspection
---
