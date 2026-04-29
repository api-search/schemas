---
description: The configuration object for Config rule evaluation mode. The Supported valid values are Detective or Proactive.
layout: schema
name: EvaluationModeConfiguration
properties_list:
- description: ''
  name: Mode
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-evaluation-mode-configuration-schema.json
slug: config-evaluation-mode-configuration
source_filename: config-evaluation-mode-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-mode-configuration-schema.json\",\n  \"title\": \"EvaluationModeConfiguration\",\n  \"description\": \"The configuration object for Config rule evaluation mode. The Supported valid values are Detective or Proactive.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMode\"\n        },\n        {\n          \"description\": \"The mode of an evaluation. The valid values are Detective or Proactive.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-mode-configuration-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: EvaluationModeConfiguration
---
