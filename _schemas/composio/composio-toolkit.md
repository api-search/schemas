---
description: Represents an application toolkit in the Composio platform, containing a collection of tools and integration metadata for a specific third-party service.
layout: schema
name: Composio Toolkit
properties_list:
- description: URL-friendly identifier for the toolkit, such as 'github', 'gmail', or 'slack'.
  name: slug
  type: string
- description: Human-readable name of the toolkit.
  name: name
  type: string
- description: Description of the toolkit and the third-party service it integrates with.
  name: description
  type: string
- description: URL of the toolkit's logo image.
  name: logo
  type: string
- description: Categories this toolkit belongs to, such as 'productivity', 'communication', or 'developer-tools'.
  name: categories
  type: array
- description: Supported authentication schemes for connecting to this toolkit.
  name: authSchemes
  type: array
- description: Number of available tools in this toolkit.
  name: toolCount
  type: integer
provider_name: Composio
provider_slug: composio
schema_file: json-schema/composio-toolkit-schema.json
slug: composio-toolkit
source_filename: composio-toolkit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://composio.dev/schemas/composio/toolkit.json\",\n  \"title\": \"Composio Toolkit\",\n  \"description\": \"Represents an application toolkit in the Composio platform, containing a collection of tools and integration metadata for a specific third-party service.\",\n  \"type\": \"object\",\n  \"required\": [\"slug\", \"name\"],\n  \"properties\": {\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly identifier for the toolkit, such as 'github', 'gmail', or 'slack'.\",\n      \"minLength\": 1,\n      \"pattern\": \"^[a-z0-9][a-z0-9-]*$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the toolkit.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the toolkit and the third-party service it integrates with.\"\n    },\n    \"logo\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the toolkit's logo image.\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"Categories this toolkit belongs to, such as 'productivity', 'communication', or 'developer-tools'.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"authSchemes\": {\n      \"type\": \"array\",\n      \"description\": \"Supported authentication schemes for connecting to this toolkit.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"OAUTH2\", \"API_KEY\", \"BASIC\", \"BEARER_TOKEN\"]\n      }\n    },\n    \"toolCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of available tools in this toolkit.\",\n      \"minimum\": 0\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/json-schema/composio-toolkit-schema.json
tags:
- AI Agents
- Authentication
- Integrations
- OAuth
- Tools
- Unified_API
title: Composio Toolkit
---
