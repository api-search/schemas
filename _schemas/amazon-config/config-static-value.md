---
description: The static value of the resource.
layout: schema
name: StaticValue
properties_list:
- description: ''
  name: Values
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-static-value-schema.json
slug: config-static-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-static-value-schema.json\",\n  \"title\": \"StaticValue\",\n  \"description\": \"The static value of the resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StaticParameterValues\"\n        },\n        {\n          \"description\": \"A list of values. For example, the ARN of the assumed role. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-static-value-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: StaticValue
---
