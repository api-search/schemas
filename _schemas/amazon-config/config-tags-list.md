---
description: TagsList schema
layout: schema
name: TagsList
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-tags-list-schema.json
slug: config-tags-list
source_filename: config-tags-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-tags-list-schema.json\",\n  \"title\": \"TagsList\",\n  \"description\": \"TagsList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Tag\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 50\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-tags-list-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: TagsList
---
