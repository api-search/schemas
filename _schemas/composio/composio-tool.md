---
description: Represents an individual tool action within a Composio toolkit, including its metadata, input parameters, and the toolkit it belongs to.
layout: schema
name: Composio Tool
properties_list:
- description: Unique identifier for the tool.
  name: id
  type: string
- description: Human-readable name of the tool.
  name: name
  type: string
- description: Description of the tool's functionality and what it does.
  name: description
  type: string
- description: The toolkit (application) this tool belongs to, such as 'github', 'gmail', or 'slack'.
  name: toolkit
  type: string
- description: JSON Schema describing the required and optional input parameters for the tool.
  name: parameters
  type: object
- description: Categorization tags for the tool.
  name: tags
  type: array
provider_name: Composio
provider_slug: composio
schema_file: json-schema/composio-tool-schema.json
slug: composio-tool
source_filename: composio-tool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://composio.dev/schemas/composio/tool.json\",\n  \"title\": \"Composio Tool\",\n  \"description\": \"Represents an individual tool action within a Composio toolkit, including its metadata, input parameters, and the toolkit it belongs to.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"toolkit\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the tool.\",\n      \"minLength\": 1\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the tool.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the tool's functionality and what it does.\"\n    },\n    \"toolkit\": {\n      \"type\": \"string\",\n      \"description\": \"The toolkit (application) this tool belongs to, such as 'github',\
  \ 'gmail', or 'slack'.\",\n      \"minLength\": 1\n    },\n    \"parameters\": {\n      \"$ref\": \"#/$defs/ParameterSchema\",\n      \"description\": \"JSON Schema describing the required and optional input parameters for the tool.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Categorization tags for the tool.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"ParameterSchema\": {\n      \"type\": \"object\",\n      \"description\": \"Schema describing the input parameters for a tool.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"object\"\n        },\n        \"required\": {\n          \"type\": \"array\",\n          \"description\": \"List of required input parameter names.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"description\"\
  : \"Map of parameter names to their type definitions.\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/ParameterDefinition\"\n          }\n        }\n      }\n    },\n    \"ParameterDefinition\": {\n      \"type\": \"object\",\n      \"description\": \"Definition of a single input parameter for a tool.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The data type of the parameter.\",\n          \"enum\": [\"string\", \"integer\", \"number\", \"boolean\", \"array\", \"object\"]\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the parameter.\"\n        },\n        \"enum\": {\n          \"type\": \"array\",\n          \"description\": \"Allowed values for the parameter.\"\n        },\n        \"default\": {\n          \"description\": \"Default value for the parameter when not provided.\"\n        },\n        \"format\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Format hint for the parameter value, such as 'email', 'uri', or 'date-time'.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/json-schema/composio-tool-schema.json
tags:
- AI Agents
- Authentication
- Integrations
- OAuth
- Tools
- Unified_API
title: Composio Tool
---
