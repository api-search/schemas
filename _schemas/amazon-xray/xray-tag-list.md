---
description: TagList schema from Amazon X-Ray API
layout: schema
name: TagList
properties_list: []
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-tag-list-schema.json
slug: xray-tag-list
source_filename: xray-tag-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Tag\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 200,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagList\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-tag-list-schema.json\",\n  \"description\": \"TagList schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-tag-list-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: TagList
---
