---
description: Guardrails configuration
layout: schema
name: GuardrailsConfig
properties_list:
- description: Controls whether guardrails are enabled
  name: enabled
  type: boolean
- description: The response when the guardrails model marks the completion as unsafe
  name: response_when_unsafe
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-inference-guardrails-config-schema.json
slug: cortex-inference-guardrails-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GuardrailsConfig\",\n  \"type\": \"object\",\n  \"description\": \"Guardrails configuration\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Controls whether guardrails are enabled\"\n    },\n    \"response_when_unsafe\": {\n      \"type\": \"string\",\n      \"description\": \"The response when the guardrails model marks the completion as unsafe\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-inference-guardrails-config-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: GuardrailsConfig
---
