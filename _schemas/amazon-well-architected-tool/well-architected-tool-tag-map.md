---
description: TagMap schema from AWS Well-Architected Tool API
layout: schema
name: TagMap
properties_list: []
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-tag-map-schema.json
slug: well-architected-tool-tag-map
source_json: "{\n  \"type\": \"object\",\n  \"minProperties\": 1,\n  \"maxProperties\": 50,\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/TagValue\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagMap\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-tag-map-schema.json\",\n  \"description\": \"TagMap schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-tag-map-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: TagMap
---
