---
description: A Postman workspace that provides an isolated environment for organizing API development work. Workspaces contain collections, environments, mock servers, monitors, and APIs, and support collaboration through shared team access.
layout: schema
name: Postman Workspace
properties_list:
- description: The workspace's unique identifier.
  name: id
  type: string
- description: The workspace name.
  name: name
  type: string
- description: The workspace type. Personal workspaces are visible only to the owner. Team workspaces are shared with all team members. Private workspaces have restricted access. Public workspaces are visible to eve
  name: type
  type: string
- description: The workspace description.
  name: description
  type: string
- description: The workspace visibility setting.
  name: visibility
  type: string
- description: The user ID of the workspace creator.
  name: createdBy
  type: string
- description: The user ID of the last person to update the workspace.
  name: updatedBy
  type: string
- description: When the workspace was created.
  name: createdAt
  type: string
- description: When the workspace was last updated.
  name: updatedAt
  type: string
- description: Collections in this workspace.
  name: collections
  type: array
- description: Environments in this workspace.
  name: environments
  type: array
- description: Mock servers in this workspace.
  name: mocks
  type: array
- description: Monitors in this workspace.
  name: monitors
  type: array
- description: APIs in this workspace.
  name: apis
  type: array
provider_name: Postman
provider_slug: postman
schema_file: json-schema/postman-workspace-schema.json
slug: postman-workspace
source_filename: postman-workspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://postman.com/schemas/postman/workspace.json\",\n  \"title\": \"Postman Workspace\",\n  \"description\": \"A Postman workspace that provides an isolated environment for organizing API development work. Workspaces contain collections, environments, mock servers, monitors, and APIs, and support collaboration through shared team access.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The workspace's unique identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The workspace name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"personal\", \"team\", \"private\", \"public\", \"partner\"],\n      \"description\": \"The workspace type. Personal workspaces are visible only to the owner. Team workspaces are shared\
  \ with all team members. Private workspaces have restricted access. Public workspaces are visible to everyone. Partner workspaces enable collaboration with external partners.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The workspace description.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"personal\", \"team\", \"private\", \"public\", \"partner\"],\n      \"description\": \"The workspace visibility setting.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the workspace creator.\"\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the last person to update the workspace.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the workspace was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"When the workspace was last updated.\"\n    },\n    \"collections\": {\n      \"type\": \"array\",\n      \"description\": \"Collections in this workspace.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/WorkspaceResource\"\n      }\n    },\n    \"environments\": {\n      \"type\": \"array\",\n      \"description\": \"Environments in this workspace.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/WorkspaceResource\"\n      }\n    },\n    \"mocks\": {\n      \"type\": \"array\",\n      \"description\": \"Mock servers in this workspace.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/WorkspaceResource\"\n      }\n    },\n    \"monitors\": {\n      \"type\": \"array\",\n      \"description\": \"Monitors in this workspace.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/WorkspaceResource\"\n      }\n    },\n    \"apis\": {\n      \"type\": \"array\",\n      \"description\": \"APIs in this workspace.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/WorkspaceResource\"\
  \n      }\n    }\n  },\n  \"$defs\": {\n    \"WorkspaceResource\": {\n      \"type\": \"object\",\n      \"description\": \"A resource linked to the workspace.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The resource's unique ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The resource name.\"\n        },\n        \"uid\": {\n          \"type\": \"string\",\n          \"description\": \"The resource's UID.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/json-schema/postman-workspace-schema.json
tags:
- AI Agent Builder
- API Development
- API Documentation
- API Governance
- API Monitoring
- API Testing
- Automation
- Client
- Clients
- Collaboration
- Collections
- Discovery
- Environments
- MCP
- Mock Servers
- Mocking
- Network
- Platform
- Testing
- Workflows
- Workspaces
title: Postman Workspace
---
