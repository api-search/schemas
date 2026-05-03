---
description: Represents a Workato AI agent (genie) — an entity that uses large language models and recipe-backed skills to autonomously handle tasks and answer questions. Genies are configured with instructions, an AI provider, skills, and knowledge bases.
layout: schema
name: Workato Genie
properties_list:
- description: Unique integer identifier of the genie within the workspace.
  name: id
  type: integer
- description: Display name of the genie.
  name: name
  type: string
- description: Human-readable description of the genie's purpose and capabilities.
  name: description
  type: string
- description: ID of the workspace folder that contains this genie.
  name: folder_id
  type: integer
- description: Current operational state of the genie.
  name: state
  type: string
- description: Natural language instructions that define the genie's behavior, persona, and decision-making approach.
  name: instructions
  type: string
- description: The AI model provider powering this genie (e.g., openai, anthropic, workato).
  name: ai_provider
  type: string
- description: ID of the shared account providing credentials for the AI provider.
  name: shared_account_id
  type: integer
- description: ID of the custom OAuth profile used for AI provider authentication.
  name: custom_oauth_key_id
  type: integer
- description: Advanced configuration settings for the genie's behavior and model parameters.
  name: matrix
  type: object
- description: List of skills (recipe-backed tools) assigned to this genie.
  name: skills
  type: array
- description: List of knowledge bases assigned to this genie for contextual data retrieval.
  name: knowledge_bases
  type: array
- description: Identity provider user groups that have access to interact with this genie.
  name: user_groups
  type: array
- description: ISO 8601 timestamp when the genie was created.
  name: created_at
  type: string
- description: ISO 8601 timestamp when the genie was last updated.
  name: updated_at
  type: string
provider_name: Workato
provider_slug: workato
schema_file: json-schema/workato-genie-schema.json
slug: workato-genie
source_filename: workato-genie-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.workato.com/schemas/genie.json\",\n  \"title\": \"Workato Genie\",\n  \"description\": \"Represents a Workato AI agent (genie) — an entity that uses large language models and recipe-backed skills to autonomously handle tasks and answer questions. Genies are configured with instructions, an AI provider, skills, and knowledge bases.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique integer identifier of the genie within the workspace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the genie.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the genie's purpose and capabilities.\"\n    },\n    \"folder_id\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"ID of the workspace folder that contains this genie.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational state of the genie.\",\n      \"enum\": [\"running\", \"stopped\"]\n    },\n    \"instructions\": {\n      \"type\": \"string\",\n      \"description\": \"Natural language instructions that define the genie's behavior, persona, and decision-making approach.\"\n    },\n    \"ai_provider\": {\n      \"type\": \"string\",\n      \"description\": \"The AI model provider powering this genie (e.g., openai, anthropic, workato).\"\n    },\n    \"shared_account_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the shared account providing credentials for the AI provider.\"\n    },\n    \"custom_oauth_key_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the custom OAuth profile used for AI provider authentication.\"\n    },\n    \"matrix\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Advanced configuration settings for the genie's behavior and model parameters.\",\n      \"additionalProperties\": true\n    },\n    \"skills\": {\n      \"type\": \"array\",\n      \"description\": \"List of skills (recipe-backed tools) assigned to this genie.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SkillRef\"\n      }\n    },\n    \"knowledge_bases\": {\n      \"type\": \"array\",\n      \"description\": \"List of knowledge bases assigned to this genie for contextual data retrieval.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/KnowledgeBaseRef\"\n      }\n    },\n    \"user_groups\": {\n      \"type\": \"array\",\n      \"description\": \"Identity provider user groups that have access to interact with this genie.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/UserGroupRef\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601\
  \ timestamp when the genie was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the genie was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"SkillRef\": {\n      \"type\": \"object\",\n      \"title\": \"Skill Reference\",\n      \"description\": \"A reference to a skill assigned to a genie.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of the skill.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the skill.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the capability this skill provides the genie.\"\n        },\n        \"recipe_id\": {\n          \"type\": \"integer\",\n          \"description\": \"ID of the underlying recipe\
  \ that implements this skill.\"\n        }\n      }\n    },\n    \"KnowledgeBaseRef\": {\n      \"type\": \"object\",\n      \"title\": \"Knowledge Base Reference\",\n      \"description\": \"A reference to a knowledge base assigned to a genie.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of the knowledge base.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the knowledge base.\"\n        },\n        \"source_type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of data sources used in the knowledge base.\"\n        }\n      }\n    },\n    \"UserGroupRef\": {\n      \"type\": \"object\",\n      \"title\": \"User Group Reference\",\n      \"description\": \"A reference to an identity provider user group.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n\
  \          \"type\": \"integer\",\n          \"description\": \"Unique identifier of the user group.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the user group.\"\n        }\n      }\n    },\n    \"DataSource\": {\n      \"type\": \"object\",\n      \"title\": \"Data Source\",\n      \"description\": \"A configured data source that feeds information into a knowledge base.\",\n      \"required\": [\"source_type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of the data source.\"\n        },\n        \"source_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of data source.\",\n          \"enum\": [\"document\", \"table\", \"api\", \"database\", \"web\"]\n        },\n        \"connection_id\": {\n          \"type\": \"integer\",\n          \"description\": \"ID of the Workato connection used to authenticate to\
  \ the data source.\"\n        },\n        \"config\": {\n          \"type\": \"object\",\n          \"description\": \"Source-specific configuration including paths, queries, or selectors.\",\n          \"additionalProperties\": true\n        },\n        \"sync_frequency\": {\n          \"type\": \"string\",\n          \"description\": \"How often the data source is synchronized.\",\n          \"enum\": [\"manual\", \"hourly\", \"daily\", \"weekly\"]\n        }\n      }\n    },\n    \"McpServer\": {\n      \"type\": \"object\",\n      \"title\": \"MCP Server\",\n      \"description\": \"A Model Context Protocol server that exposes Workato API collections as tools for external AI agents.\",\n      \"required\": [\"handle\", \"name\"],\n      \"properties\": {\n        \"handle\": {\n          \"type\": \"string\",\n          \"description\": \"Unique slug identifier of the MCP server.\",\n          \"pattern\": \"^[a-z0-9-]+$\"\n        },\n        \"name\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Display name of the MCP server.\",\n          \"minLength\": 1,\n          \"maxLength\": 255\n        },\n        \"folder_id\": {\n          \"type\": \"integer\",\n          \"description\": \"ID of the folder containing this MCP server.\"\n        },\n        \"mcp_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The authenticated MCP URL for AI agents to connect to.\"\n        },\n        \"authentication_method\": {\n          \"type\": \"string\",\n          \"description\": \"Authentication method used by the MCP server.\"\n        },\n        \"tools\": {\n          \"type\": \"array\",\n          \"description\": \"List of tools (API endpoints) exposed through this MCP server.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/McpTool\"\n          }\n        },\n        \"policies\": {\n          \"$ref\": \"#/$defs/ServerPolicy\"\n        },\n        \"created_at\": {\n          \"\
  type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the MCP server was created.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the MCP server was last updated.\"\n        }\n      }\n    },\n    \"McpTool\": {\n      \"type\": \"object\",\n      \"title\": \"MCP Tool\",\n      \"description\": \"An individual API endpoint exposed as a callable tool through an MCP server.\",\n      \"required\": [\"id\", \"trigger_application\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the tool within its application.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the tool shown to AI agents.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n       \
  \   \"description\": \"Description of what the tool does and when AI agents should use it.\"\n        },\n        \"trigger_application\": {\n          \"type\": \"string\",\n          \"description\": \"The application or API collection that owns this tool.\"\n        }\n      }\n    },\n    \"ServerPolicy\": {\n      \"type\": \"object\",\n      \"title\": \"Server Policy\",\n      \"description\": \"Security and rate limiting policies for an MCP server.\",\n      \"properties\": {\n        \"rate_limit\": {\n          \"type\": \"object\",\n          \"description\": \"Rate limiting configuration.\",\n          \"properties\": {\n            \"requests_per_minute\": {\n              \"type\": \"integer\",\n              \"minimum\": 1,\n              \"description\": \"Maximum requests allowed per minute.\"\n            },\n            \"requests_per_hour\": {\n              \"type\": \"integer\",\n              \"minimum\": 1,\n              \"description\": \"Maximum requests allowed\
  \ per hour.\"\n            }\n          }\n        },\n        \"quota_limit\": {\n          \"type\": \"object\",\n          \"description\": \"Monthly quota configuration.\",\n          \"properties\": {\n            \"requests_per_month\": {\n              \"type\": \"integer\",\n              \"minimum\": 1,\n              \"description\": \"Maximum requests allowed per month.\"\n            }\n          }\n        },\n        \"ip_allowlist\": {\n          \"type\": \"array\",\n          \"description\": \"IP addresses or CIDR ranges permitted to access the server.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"IP address or CIDR range.\"\n          }\n        },\n        \"ip_denylist\": {\n          \"type\": \"array\",\n          \"description\": \"IP addresses or CIDR ranges blocked from accessing the server.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"IP address or CIDR range.\"\n\
  \          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/json-schema/workato-genie-schema.json
tags:
- Agentic
- API Management
- Automation
- B2B
- Embedded iPaaS
- Enterprise
- Integration
- iPaaS
- Orchestration
- Workflow
title: Workato Genie
---
