---
description: Represents an API operation or workflow in the Jentic catalog, including its metadata, input schema, and execution requirements.
layout: schema
name: Jentic Operation
properties_list:
- description: Unique identifier for the operation, prefixed with 'op_' for operations or 'wf_' for workflows.
  name: uuid
  type: string
- description: Human-readable name of the operation or workflow.
  name: name
  type: string
- description: Detailed description of what the operation or workflow does.
  name: description
  type: string
- description: Whether this is a single API operation or a multi-step Arazzo workflow.
  name: type
  type: string
- description: Name of the upstream API that provides this operation.
  name: api_name
  type: string
- description: HTTP method for the operation, applicable to single operations.
  name: method
  type: string
- description: URL path template for the operation.
  name: path
  type: string
- description: JSON Schema describing the required and optional input parameters.
  name: inputs
  type: object
- description: Whether upstream API credentials must be configured in the Jentic credential vault.
  name: auth_required
  type: boolean
- description: Categorization tags for the operation.
  name: tags
  type: array
provider_name: Jentic
provider_slug: jentic
schema_file: json-schema/jentic-operation-schema.json
slug: jentic-operation
source_filename: jentic-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jentic.com/schemas/jentic/operation.json\",\n  \"title\": \"Jentic Operation\",\n  \"description\": \"Represents an API operation or workflow in the Jentic catalog, including its metadata, input schema, and execution requirements.\",\n  \"type\": \"object\",\n  \"required\": [\"uuid\", \"name\", \"type\"],\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the operation, prefixed with 'op_' for operations or 'wf_' for workflows.\",\n      \"pattern\": \"^(op_|wf_).+\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the operation or workflow.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of what the operation or workflow does.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Whether this is a single API operation or a multi-step Arazzo workflow.\",\n      \"enum\": [\"operation\", \"workflow\"]\n    },\n    \"api_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the upstream API that provides this operation.\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP method for the operation, applicable to single operations.\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\"]\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"URL path template for the operation.\"\n    },\n    \"inputs\": {\n      \"$ref\": \"#/$defs/InputSchema\",\n      \"description\": \"JSON Schema describing the required and optional input parameters.\"\n    },\n    \"auth_required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether upstream API credentials must be configured in the Jentic credential vault.\",\n      \"default\": false\n    },\n\
  \    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Categorization tags for the operation.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"InputSchema\": {\n      \"type\": \"object\",\n      \"description\": \"Schema describing the input parameters for an operation.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"object\"\n        },\n        \"required\": {\n          \"type\": \"array\",\n          \"description\": \"List of required input parameter names.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"description\": \"Map of parameter names to their type definitions.\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/InputParameter\"\n          }\n        }\n      }\n    },\n    \"InputParameter\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Definition of a single input parameter for an operation.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The data type of the parameter.\",\n          \"enum\": [\"string\", \"integer\", \"number\", \"boolean\", \"array\", \"object\"]\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the parameter.\"\n        },\n        \"enum\": {\n          \"type\": \"array\",\n          \"description\": \"Allowed values for the parameter.\"\n        },\n        \"default\": {\n          \"description\": \"Default value for the parameter when not provided.\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"description\": \"Format hint for the parameter value, such as 'email', 'uri', or 'date-time'.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jentic/refs/heads/main/json-schema/jentic-operation-schema.json
tags:
- AI Agents
- Arazzo
- Integrations
- MCP
- OpenAPI
- Workflows
title: Jentic Operation
---
