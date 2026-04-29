---
description: NewRecInspection schema from 1Factory API
layout: schema
name: NewRecInspection
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-new-rec-inspection-schema.json
slug: 1factory-new-rec-inspection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-new-rec-inspection-schema.json\",\n  \"title\": \"NewRecInspection\",\n  \"description\": \"NewRecInspection schema from 1Factory API\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/NewInspection\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"supplier_name\": {\n          \"$ref\": \"#/components/schemas/supplier_name\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-new-rec-inspection-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: NewRecInspection
---
