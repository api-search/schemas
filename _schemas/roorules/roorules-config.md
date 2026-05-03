---
description: Schema for Roo Code AI coding assistant configuration including .roorules file format, custom modes, and API configuration profiles.
layout: schema
name: Roo Code Configuration Schema
properties_list:
- description: Array of custom mode definitions for the Roo Code instance
  name: customModes
  type: array
- description: Array of API configuration profiles
  name: apiProfiles
  type: array
- description: Named MCP server configurations
  name: mcpServers
  type: object
provider_name: .Roorules
provider_slug: roorules
schema_file: json-schema/roorules-config-schema.json
slug: roorules-config
source_filename: roorules-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://roocode.com/schemas/roorules-config.json\",\n  \"title\": \"Roo Code Configuration Schema\",\n  \"description\": \"Schema for Roo Code AI coding assistant configuration including .roorules file format, custom modes, and API configuration profiles.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"RooruleFile\": {\n      \"type\": \"object\",\n      \"title\": \"RooruleFile\",\n      \"description\": \"A .roorules project configuration file providing instructions for Roo Code AI agents\",\n      \"properties\": {\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"Free-form text or Markdown content containing coding conventions, style guidelines, and behavioral instructions for Roo Code agents\"\n        }\n      }\n    },\n    \"CustomMode\": {\n      \"type\": \"object\",\n      \"title\": \"CustomMode\",\n      \"description\": \"A custom Roo Code\
  \ operational mode defined in .roomodes\",\n      \"required\": [\"slug\", \"name\", \"roleDefinition\"],\n      \"properties\": {\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the mode in kebab-case\",\n          \"pattern\": \"^[a-z][a-z0-9-]*$\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable display name for the mode\"\n        },\n        \"roleDefinition\": {\n          \"type\": \"string\",\n          \"description\": \"System prompt text defining the role, capabilities, and constraints of this mode\"\n        },\n        \"groups\": {\n          \"type\": \"array\",\n          \"description\": \"Tool groups this mode is allowed to use\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"read\", \"edit\", \"browser\", \"command\", \"mcp\"]\n          }\n        },\n        \"customInstructions\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Additional mode-specific instructions appended to the system prompt\"\n        }\n      }\n    },\n    \"ApiConfigurationProfile\": {\n      \"type\": \"object\",\n      \"title\": \"ApiConfigurationProfile\",\n      \"description\": \"A saved AI provider and model configuration profile for Roo Code\",\n      \"required\": [\"id\", \"name\", \"apiProvider\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the profile\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name for the profile\"\n        },\n        \"apiProvider\": {\n          \"type\": \"string\",\n          \"description\": \"AI provider identifier\",\n          \"enum\": [\"anthropic\", \"openai\", \"google\", \"bedrock\", \"openrouter\", \"ollama\", \"lmstudio\", \"mistral\", \"deepseek\", \"xai\"]\n        },\n        \"apiModelId\": {\n       \
  \   \"type\": \"string\",\n          \"description\": \"Model identifier for the selected provider (e.g., claude-3-7-sonnet-20250219)\"\n        },\n        \"apiKey\": {\n          \"type\": \"string\",\n          \"description\": \"API key for the provider (stored securely, not in files)\"\n        }\n      }\n    },\n    \"McpServerConfig\": {\n      \"type\": \"object\",\n      \"title\": \"McpServerConfig\",\n      \"description\": \"Configuration for an MCP server connected to Roo Code\",\n      \"required\": [\"command\"],\n      \"properties\": {\n        \"command\": {\n          \"type\": \"string\",\n          \"description\": \"Command to launch the MCP server process\"\n        },\n        \"args\": {\n          \"type\": \"array\",\n          \"description\": \"Arguments passed to the MCP server command\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"env\": {\n          \"type\": \"object\",\n          \"description\": \"Environment variables set\
  \ for the MCP server process\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"disabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this MCP server is currently disabled\",\n          \"default\": false\n        }\n      }\n    }\n  },\n  \"properties\": {\n    \"customModes\": {\n      \"type\": \"array\",\n      \"description\": \"Array of custom mode definitions for the Roo Code instance\",\n      \"items\": { \"$ref\": \"#/$defs/CustomMode\" }\n    },\n    \"apiProfiles\": {\n      \"type\": \"array\",\n      \"description\": \"Array of API configuration profiles\",\n      \"items\": { \"$ref\": \"#/$defs/ApiConfigurationProfile\" }\n    },\n    \"mcpServers\": {\n      \"type\": \"object\",\n      \"description\": \"Named MCP server configurations\",\n      \"additionalProperties\": { \"$ref\": \"#/$defs/McpServerConfig\" }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/roorules/refs/heads/main/json-schema/roorules-config-schema.json
tags:
- AI Agents
- AI Copilot
- Coding Assistant
- Coding Standards
- Developer Workflow
- LLM
- MCP
- Roo Code
- VS Code
title: Roo Code Configuration Schema
---
