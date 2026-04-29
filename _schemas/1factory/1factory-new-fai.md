---
description: NewFai schema from 1Factory API
layout: schema
name: NewFai
properties_list:
- description: ''
  name: insp_ident_1
  type: object
- description: ''
  name: insp_ident_2
  type: object
- description: ''
  name: part_number
  type: object
- description: ''
  name: rev
  type: object
- description: ''
  name: fai_type
  type: object
- description: ''
  name: number_of_parts
  type: object
- description: ''
  name: customer_name
  type: object
- description: ''
  name: supplier_name
  type: object
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-new-fai-schema.json
slug: 1factory-new-fai
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-new-fai-schema.json\",\n  \"title\": \"NewFai\",\n  \"description\": \"NewFai schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"insp_ident_1\": {\n      \"$ref\": \"#/components/schemas/insp_ident_1\"\n    },\n    \"insp_ident_2\": {\n      \"$ref\": \"#/components/schemas/insp_ident_2\"\n    },\n    \"part_number\": {\n      \"$ref\": \"#/components/schemas/part_number\"\n    },\n    \"rev\": {\n      \"$ref\": \"#/components/schemas/rev\"\n    },\n    \"fai_type\": {\n      \"$ref\": \"#/components/schemas/fai_type\"\n    },\n    \"number_of_parts\": {\n      \"$ref\": \"#/components/schemas/number_of_parts\"\n    },\n    \"customer_name\": {\n      \"$ref\": \"#/components/schemas/customer_name\"\n    },\n    \"supplier_name\": {\n      \"$ref\": \"#/components/schemas/supplier_name\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-new-fai-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: NewFai
---
