---
description: ResourceKeys schema
layout: schema
name: ResourceKeys
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-resource-keys-schema.json
slug: config-resource-keys
source_filename: config-resource-keys-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-keys-schema.json\",\n  \"title\": \"ResourceKeys\",\n  \"description\": \"ResourceKeys schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ResourceKey\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 100\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-keys-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ResourceKeys
---
