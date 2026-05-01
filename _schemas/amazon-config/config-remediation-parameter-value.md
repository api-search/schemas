---
description: The value is either a dynamic (resource) value or a static value. You must select either a dynamic value or a static value.
layout: schema
name: RemediationParameterValue
properties_list:
- description: ''
  name: ResourceValue
  type: object
- description: ''
  name: StaticValue
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-remediation-parameter-value-schema.json
slug: config-remediation-parameter-value
source_filename: config-remediation-parameter-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-remediation-parameter-value-schema.json\",\n  \"title\": \"RemediationParameterValue\",\n  \"description\": \"The value is either a dynamic (resource) value or a static value. You must select either a dynamic value or a static value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceValue\"\n        },\n        {\n          \"description\": \"The value is dynamic and changes at run-time.\"\n        }\n      ]\n    },\n    \"StaticValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StaticValue\"\n        },\n        {\n          \"description\": \"The value is static and does not change at run-time.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-remediation-parameter-value-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: RemediationParameterValue
---
