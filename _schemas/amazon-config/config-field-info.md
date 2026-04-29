---
description: Details about the fields such as name of the field.
layout: schema
name: FieldInfo
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-field-info-schema.json
slug: config-field-info
source_filename: config-field-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-field-info-schema.json\",\n  \"title\": \"FieldInfo\",\n  \"description\": \"Details about the fields such as name of the field.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FieldName\"\n        },\n        {\n          \"description\": \"Name of the field.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-field-info-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: FieldInfo
---
