---
description: ControlsList schema
layout: schema
name: ControlsList
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-controls-list-schema.json
slug: config-controls-list
source_filename: config-controls-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-controls-list-schema.json\",\n  \"title\": \"ControlsList\",\n  \"description\": \"ControlsList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/StringWithCharLimit128\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 20\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-controls-list-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ControlsList
---
