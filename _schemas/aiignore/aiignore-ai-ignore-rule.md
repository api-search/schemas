---
description: A single .aiignore exclusion rule pattern with metadata
layout: schema
name: AIIgnoreRule
properties_list:
- description: Glob pattern for matching files/directories
  name: pattern
  type: string
- description: Human-readable explanation of this rule
  name: comment
  type: string
- description: If true, this rule re-includes a previously excluded path (starts with !)
  name: negated
  type: boolean
- description: 'Scope: file, directory, or pattern'
  name: scope
  type: string
provider_name: .AIIgnore
provider_slug: aiignore
schema_file: json-schema/aiignore-ai-ignore-rule-schema.json
slug: aiignore-ai-ignore-rule
source_filename: aiignore-ai-ignore-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aiignore/refs/heads/main/json-schema/aiignore-ai-ignore-rule-schema.json\",\n  \"title\": \"AIIgnoreRule\",\n  \"description\": \"A single .aiignore exclusion rule pattern with metadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pattern\": {\n      \"type\": \"string\",\n      \"description\": \"Glob pattern for matching files/directories\",\n      \"example\": \"**/.env\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable explanation of this rule\",\n      \"example\": \"Exclude environment files with secrets\"\n    },\n    \"negated\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, this rule re-includes a previously excluded path (starts with !)\",\n      \"example\": false\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Scope: file,\
  \ directory, or pattern\",\n      \"example\": \"file\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aiignore/refs/heads/main/json-schema/aiignore-ai-ignore-rule-schema.json
tags:
- AI Agents
- Configuration
- Developer Workflow
- Security
- Privacy
- Developer Tools
- LLM
- Secrets Management
title: AIIgnoreRule
---
