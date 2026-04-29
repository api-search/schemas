---
description: TagKeyList schema from Amazon X-Ray API
layout: schema
name: TagKeyList
properties_list: []
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-tag-key-list-schema.json
slug: xray-tag-key-list
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/TagKey\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 200,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagKeyList\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-tag-key-list-schema.json\",\n  \"description\": \"TagKeyList schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-tag-key-list-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: TagKeyList
---
