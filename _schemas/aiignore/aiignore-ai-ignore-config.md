---
description: Full .aiignore configuration file structure for an AI coding tool
layout: schema
name: AIIgnoreConfig
properties_list:
- description: Target AI tool this config applies to
  name: tool
  type: string
- description: AIIgnore spec version
  name: version
  type: string
- description: List of exclusion rules
  name: rules
  type: array
- description: Human-readable description of this config purpose
  name: description
  type: string
provider_name: .AIIgnore
provider_slug: aiignore
schema_file: json-schema/aiignore-ai-ignore-config-schema.json
slug: aiignore-ai-ignore-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aiignore/refs/heads/main/json-schema/aiignore-ai-ignore-config-schema.json\",\n  \"title\": \"AIIgnoreConfig\",\n  \"description\": \"Full .aiignore configuration file structure for an AI coding tool\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tool\": {\n      \"type\": \"string\",\n      \"description\": \"Target AI tool this config applies to\",\n      \"example\": \"jetbrains\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"AIIgnore spec version\",\n      \"example\": \"1.0\"\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"List of exclusion rules\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of this config purpose\",\n      \"example\"\
  : \"Protect secrets and proprietary code from AI coding tools\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aiignore/refs/heads/main/json-schema/aiignore-ai-ignore-config-schema.json
tags:
- AI Agents
- Configuration
- Developer Workflow
- Security
- Privacy
- Developer Tools
- LLM
- Secrets Management
title: AIIgnoreConfig
---
