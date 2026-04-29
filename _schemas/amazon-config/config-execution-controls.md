---
description: The controls that Config uses for executing remediations.
layout: schema
name: ExecutionControls
properties_list:
- description: ''
  name: SsmControls
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-execution-controls-schema.json
slug: config-execution-controls
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-execution-controls-schema.json\",\n  \"title\": \"ExecutionControls\",\n  \"description\": \"The controls that Config uses for executing remediations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SsmControls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SsmControls\"\n        },\n        {\n          \"description\": \"A SsmControls object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-execution-controls-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ExecutionControls
---
