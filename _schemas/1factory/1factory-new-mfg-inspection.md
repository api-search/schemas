---
description: NewMfgInspection schema from 1Factory API
layout: schema
name: NewMfgInspection
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-new-mfg-inspection-schema.json
slug: 1factory-new-mfg-inspection
source_filename: 1factory-new-mfg-inspection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-new-mfg-inspection-schema.json\",\n  \"title\": \"NewMfgInspection\",\n  \"description\": \"NewMfgInspection schema from 1Factory API\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/NewInspection\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"customer_name\": {\n          \"$ref\": \"#/components/schemas/customer_name\"\n        },\n        \"machines\": {\n          \"$ref\": \"#/components/schemas/machines\"\n        },\n        \"operation\": {\n          \"$ref\": \"#/components/schemas/operation\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-new-mfg-inspection-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: NewMfgInspection
---
