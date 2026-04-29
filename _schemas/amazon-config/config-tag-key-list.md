---
description: TagKeyList schema
layout: schema
name: TagKeyList
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-tag-key-list-schema.json
slug: config-tag-key-list
source_filename: config-tag-key-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-tag-key-list-schema.json\",\n  \"title\": \"TagKeyList\",\n  \"description\": \"TagKeyList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/TagKey\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 50\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-tag-key-list-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: TagKeyList
---
