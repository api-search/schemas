---
description: SpecInspectionType schema from 1Factory API
layout: schema
name: SpecInspectionType
properties_list:
- description: ''
  name: inspection_type
  type: object
- description: How the feature should be inspected.
  name: inspection_method
  type: string
- description: How frequently should the feature be checked.
  name: sampling_rule
  type: string
- description: How the data for this specification is recorded - numerically, as a pass/fail, or calculated from other features.
  name: data_type
  type: string
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-spec-inspection-type-schema.json
slug: 1factory-spec-inspection-type
source_filename: 1factory-spec-inspection-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-spec-inspection-type-schema.json\",\n  \"title\": \"SpecInspectionType\",\n  \"description\": \"SpecInspectionType schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inspection_type\": {\n      \"$ref\": \"#/components/schemas/inspection_type\"\n    },\n    \"inspection_method\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"How the feature should be inspected.\",\n      \"example\": \"CMM\"\n    },\n    \"sampling_rule\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"How frequently should the feature be checked.\",\n      \"example\": \"1 in 10\"\n    },\n    \"data_type\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"enum\": [\n        \"NUM\",\n        \"P/F\",\n       \
  \ \"CALC\"\n      ],\n      \"description\": \"How the data for this specification is recorded - numerically, as a pass/fail, or calculated from other features.\",\n      \"example\": \"NUM\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-spec-inspection-type-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: SpecInspectionType
---
