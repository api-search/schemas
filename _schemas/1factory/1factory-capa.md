---
description: Capa schema from 1Factory API
layout: schema
name: Capa
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-capa-schema.json
slug: 1factory-capa
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-capa-schema.json\",\n  \"title\": \"Capa\",\n  \"description\": \"Capa schema from 1Factory API\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Issue\"\n    },\n    {\n      \"properties\": {\n        \"date_due\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date & time that a CAPA is due.\",\n          \"example\": \"2021-07-21T07:14:42-08:00\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-capa-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Capa
---
