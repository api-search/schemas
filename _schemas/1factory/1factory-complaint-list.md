---
description: ComplaintList schema from 1Factory API
layout: schema
name: ComplaintList
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-complaint-list-schema.json
slug: 1factory-complaint-list
source_filename: 1factory-complaint-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-complaint-list-schema.json\",\n  \"title\": \"ComplaintList\",\n  \"description\": \"ComplaintList schema from 1Factory API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Complaint\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 500\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-complaint-list-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: ComplaintList
---
