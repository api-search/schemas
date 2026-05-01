---
description: TagList schema
layout: schema
name: TagList
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-tag-list-schema.json
slug: config-tag-list
source_filename: config-tag-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-tag-list-schema.json\",\n  \"title\": \"TagList\",\n  \"description\": \"TagList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Tag\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 50\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-tag-list-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: TagList
---
