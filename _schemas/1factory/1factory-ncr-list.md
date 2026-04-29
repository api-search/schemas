---
description: NcrList schema from 1Factory API
layout: schema
name: NcrList
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-ncr-list-schema.json
slug: 1factory-ncr-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-ncr-list-schema.json\",\n  \"title\": \"NcrList\",\n  \"description\": \"NcrList schema from 1Factory API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Ncr\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 500\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-ncr-list-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: NcrList
---
