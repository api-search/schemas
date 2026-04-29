---
description: A pattern category for AI ignore exclusion rules
layout: schema
name: ExclusionPattern
properties_list:
- description: Category name (secrets, proprietary, generated)
  name: category
  type: string
- description: List of glob patterns in this category
  name: patterns
  type: array
- description: Why these files should be excluded
  name: rationale
  type: string
provider_name: .AIIgnore
provider_slug: aiignore
schema_file: json-schema/aiignore-exclusion-pattern-schema.json
slug: aiignore-exclusion-pattern
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aiignore/refs/heads/main/json-schema/aiignore-exclusion-pattern-schema.json\",\n  \"title\": \"ExclusionPattern\",\n  \"description\": \"A pattern category for AI ignore exclusion rules\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category name (secrets, proprietary, generated)\",\n      \"example\": \"secrets\"\n    },\n    \"patterns\": {\n      \"type\": \"array\",\n      \"description\": \"List of glob patterns in this category\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"rationale\": {\n      \"type\": \"string\",\n      \"description\": \"Why these files should be excluded\",\n      \"example\": \"Contains API keys and credentials that should not be sent to AI APIs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aiignore/refs/heads/main/json-schema/aiignore-exclusion-pattern-schema.json
tags:
- AI Agents
- Configuration
- Developer Workflow
- Security
- Privacy
- Developer Tools
- LLM
- Secrets Management
title: ExclusionPattern
---
