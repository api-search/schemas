---
description: Represents an AI agent in the Toolhouse platform, including its configuration, tools, schedules, and execution metadata.
layout: schema
name: Toolhouse Agent
properties_list:
- description: Unique identifier for the agent (UUID format).
  name: agentId
  type: string
- description: Human-readable name of the agent.
  name: name
  type: string
- description: Detailed description of what the agent does.
  name: description
  type: string
- description: The type of entity this schema represents.
  name: type
  type: string
- description: URL-friendly vanity slug for the agent.
  name: slug
  type: string
- description: The LLM model used by the agent (e.g., gpt-4, claude-3).
  name: model
  type: string
- description: System prompt that defines the agent's behavior and personality.
  name: system_prompt
  type: string
- description: Whether the agent is publicly accessible without authentication.
  name: is_public
  type: boolean
- description: Collection of tools available to the agent.
  name: tools
  type: object
- description: Tool bundles assigned to the agent.
  name: bundles
  type: array
- description: Files attached to the agent for RAG or reference.
  name: files
  type: array
- description: Scheduled execution configuration for the agent.
  name: schedule
  type: object
- description: Whether Bearer token authentication is required to invoke the agent.
  name: auth_required
  type: boolean
- description: Categorization tags for the agent.
  name: tags
  type: array
- description: Visual theme customization for the agent.
  name: theme
  type: object
- description: Monetization settings for the agent.
  name: monetization
  type: object
provider_name: Toolhouse
provider_slug: toolhouse
schema_file: json-schema/toolhouse-agent-schema.json
slug: toolhouse-agent
source_filename: toolhouse-agent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://toolhouse.ai/schemas/toolhouse/agent.json\",\n  \"title\": \"Toolhouse Agent\",\n  \"description\": \"Represents an AI agent in the Toolhouse platform, including its configuration, tools, schedules, and execution metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"agentId\", \"name\", \"type\"],\n  \"properties\": {\n    \"agentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the agent (UUID format).\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the agent.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of what the agent does.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of entity this schema represents.\",\n      \"enum\": [\"\
  agent\", \"tool\", \"schedule\", \"bundle\"]\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly vanity slug for the agent.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The LLM model used by the agent (e.g., gpt-4, claude-3).\"\n    },\n    \"system_prompt\": {\n      \"type\": \"string\",\n      \"description\": \"System prompt that defines the agent's behavior and personality.\"\n    },\n    \"is_public\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the agent is publicly accessible without authentication.\",\n      \"default\": false\n    },\n    \"tools\": {\n      \"$ref\": \"#/$defs/ToolSet\",\n      \"description\": \"Collection of tools available to the agent.\"\n    },\n    \"bundles\": {\n      \"type\": \"array\",\n      \"description\": \"Tool bundles assigned to the agent.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Bundle\"\n      }\n    },\n    \"files\": {\n     \
  \ \"type\": \"array\",\n      \"description\": \"Files attached to the agent for RAG or reference.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AgentFile\"\n      }\n    },\n    \"schedule\": {\n      \"$ref\": \"#/$defs/Schedule\",\n      \"description\": \"Scheduled execution configuration for the agent.\"\n    },\n    \"auth_required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Bearer token authentication is required to invoke the agent.\",\n      \"default\": true\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Categorization tags for the agent.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"theme\": {\n      \"$ref\": \"#/$defs/ThemePreference\",\n      \"description\": \"Visual theme customization for the agent.\"\n    },\n    \"monetization\": {\n      \"$ref\": \"#/$defs/Monetization\",\n      \"description\": \"Monetization settings for the agent.\"\n    }\n  },\n  \"$defs\": {\n    \"\
  ToolSet\": {\n      \"type\": \"object\",\n      \"description\": \"A collection of tools available to an agent.\",\n      \"properties\": {\n        \"installed\": {\n          \"type\": \"array\",\n          \"description\": \"List of tools installed and available for the agent.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Tool\"\n          }\n        }\n      }\n    },\n    \"Tool\": {\n      \"type\": \"object\",\n      \"description\": \"A single tool that can be executed by an agent.\",\n      \"required\": [\"toolId\", \"name\"],\n      \"properties\": {\n        \"toolId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the tool.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name of the tool.\",\n          \"minLength\": 1\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of what the tool does.\"\
  \n        },\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"Category the tool belongs to.\"\n        },\n        \"inputs\": {\n          \"$ref\": \"#/$defs/InputSchema\",\n          \"description\": \"JSON Schema describing the tool's input parameters.\"\n        }\n      }\n    },\n    \"Bundle\": {\n      \"type\": \"object\",\n      \"description\": \"A named collection of tools grouped together.\",\n      \"required\": [\"bundleId\", \"name\"],\n      \"properties\": {\n        \"bundleId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the bundle.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the bundle.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the bundle's purpose.\"\n        },\n        \"tools\": {\n          \"type\": \"array\",\n          \"description\": \"\
  Tools included in this bundle.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Tool\"\n          }\n        }\n      }\n    },\n    \"AgentFile\": {\n      \"type\": \"object\",\n      \"description\": \"A file attached to an agent.\",\n      \"required\": [\"fileId\"],\n      \"properties\": {\n        \"fileId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the file.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"File name.\"\n        },\n        \"position\": {\n          \"type\": \"integer\",\n          \"description\": \"Display position of the file.\"\n        }\n      }\n    },\n    \"Schedule\": {\n      \"type\": \"object\",\n      \"description\": \"Scheduled execution configuration using cron expressions.\",\n      \"properties\": {\n        \"scheduleId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the schedule.\"\n        },\n\
  \        \"cron_expression\": {\n          \"type\": \"string\",\n          \"description\": \"Cron expression defining the execution schedule.\"\n        },\n        \"is_active\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the schedule is currently active.\",\n          \"default\": true\n        }\n      }\n    },\n    \"ThemePreference\": {\n      \"type\": \"object\",\n      \"description\": \"Visual theme customization for the agent UI.\",\n      \"properties\": {\n        \"theme\": {\n          \"type\": \"string\",\n          \"description\": \"Theme identifier or configuration.\"\n        }\n      }\n    },\n    \"Monetization\": {\n      \"type\": \"object\",\n      \"description\": \"Monetization configuration for a paid agent.\",\n      \"properties\": {\n        \"is_monetized\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the agent charges for access.\"\n        },\n        \"price\": {\n          \"type\": \"\
  number\",\n          \"description\": \"Subscription price for the agent.\"\n        },\n        \"subscriber_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of active subscribers.\"\n        }\n      }\n    },\n    \"InputSchema\": {\n      \"type\": \"object\",\n      \"description\": \"Schema describing the input parameters for a tool or operation.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"object\"\n        },\n        \"required\": {\n          \"type\": \"array\",\n          \"description\": \"List of required input parameter names.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"description\": \"Map of parameter names to their type definitions.\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/InputParameter\"\n          }\n        }\n      }\n    },\n\
  \    \"InputParameter\": {\n      \"type\": \"object\",\n      \"description\": \"Definition of a single input parameter.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The data type of the parameter.\",\n          \"enum\": [\"string\", \"integer\", \"number\", \"boolean\", \"array\", \"object\"]\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the parameter.\"\n        },\n        \"enum\": {\n          \"type\": \"array\",\n          \"description\": \"Allowed values for the parameter.\"\n        },\n        \"default\": {\n          \"description\": \"Default value for the parameter when not provided.\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"description\": \"Format hint for the parameter value, such as 'email', 'uri', or 'date-time'.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/json-schema/toolhouse-agent-schema.json
tags:
- Agent Infrastructure
- AI Agents
- Backend as a Service
- Tools
title: Toolhouse Agent
---
