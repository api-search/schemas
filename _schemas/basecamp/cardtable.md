---
description: ''
layout: schema
name: CardTable
properties_list: []
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/cardtable-schema.json
slug: cardtable
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/cardtable-schema.json\",\n  \"title\": \"CardTable\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Recording\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"lists\": {\n          \"type\": \"array\",\n          \"description\": \"Columns in the card table\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/CardColumn\"\n          }\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/cardtable-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: CardTable
---
