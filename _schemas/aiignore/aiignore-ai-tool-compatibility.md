---
description: Compatibility record showing which AI tools support a given .aiignore syntax
layout: schema
name: AIToolCompatibility
properties_list:
- description: Name of the AI coding tool
  name: tool_name
  type: string
- description: The actual ignore file name this tool uses
  name: file_name
  type: string
- description: Ignore file syntax type
  name: syntax
  type: string
- description: Where file should be placed
  name: scope
  type: string
- description: Link to tool documentation
  name: documentation_url
  type: string
provider_name: .AIIgnore
provider_slug: aiignore
schema_file: json-schema/aiignore-ai-tool-compatibility-schema.json
slug: aiignore-ai-tool-compatibility
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aiignore/refs/heads/main/json-schema/aiignore-ai-tool-compatibility-schema.json\",\n  \"title\": \"AIToolCompatibility\",\n  \"description\": \"Compatibility record showing which AI tools support a given .aiignore syntax\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tool_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the AI coding tool\",\n      \"example\": \"JetBrains AI Assistant\"\n    },\n    \"file_name\": {\n      \"type\": \"string\",\n      \"description\": \"The actual ignore file name this tool uses\",\n      \"example\": \".aiignore\"\n    },\n    \"syntax\": {\n      \"type\": \"string\",\n      \"description\": \"Ignore file syntax type\",\n      \"example\": \"gitignore-compatible\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Where file should be placed\",\n\
  \      \"example\": \"project root\"\n    },\n    \"documentation_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Link to tool documentation\",\n      \"example\": \"https://www.jetbrains.com/help/idea/ai-assistant.html\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aiignore/refs/heads/main/json-schema/aiignore-ai-tool-compatibility-schema.json
tags:
- AI Agents
- Configuration
- Developer Workflow
- Security
- Privacy
- Developer Tools
- LLM
- Secrets Management
title: AIToolCompatibility
---
