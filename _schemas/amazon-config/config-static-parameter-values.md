---
description: StaticParameterValues schema
layout: schema
name: StaticParameterValues
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-static-parameter-values-schema.json
slug: config-static-parameter-values
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-static-parameter-values-schema.json\",\n  \"title\": \"StaticParameterValues\",\n  \"description\": \"StaticParameterValues schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 25\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-static-parameter-values-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: StaticParameterValues
---
