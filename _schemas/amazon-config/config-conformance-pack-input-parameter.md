---
description: Input parameters in the form of key-value pairs for the conformance pack, both of which you define. Keys can have a maximum character length of 255 characters, and values can have a maximum length of 4096 characters.
layout: schema
name: ConformancePackInputParameter
properties_list:
- description: ''
  name: ParameterName
  type: object
- description: ''
  name: ParameterValue
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-input-parameter-schema.json
slug: config-conformance-pack-input-parameter
source_filename: config-conformance-pack-input-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-input-parameter-schema.json\",\n  \"title\": \"ConformancePackInputParameter\",\n  \"description\": \"Input parameters in the form of key-value pairs for the conformance pack, both of which you define. Keys can have a maximum character length of 255 characters, and values can have a maximum length of 4096 characters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ParameterName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParameterName\"\n        },\n        {\n          \"description\": \"One part of a key-value pair.\"\n        }\n      ]\n    },\n    \"ParameterValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParameterValue\"\n        },\n        {\n          \"description\": \"Another part of the key-value\
  \ pair. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ParameterName\",\n    \"ParameterValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-input-parameter-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackInputParameter
---
