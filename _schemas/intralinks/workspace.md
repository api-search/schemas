---
description: A workspace (exchange or virtual data room) in the Intralinks platform used for secure document sharing and collaboration during M&A transactions, due diligence, and other confidential business processes.
layout: schema
name: Intralinks Workspace
properties_list:
- description: Unique identifier of the workspace.
  name: id
  type: string
- description: Name of the workspace.
  name: name
  type: string
- description: Type of workspace (e.g., ATC, ILP).
  name: type
  type: string
- description: Current phase of the workspace lifecycle.
  name: phase
  type: string
- description: Current status of the workspace.
  name: status
  type: string
- description: Host organization name.
  name: host
  type: string
- description: Workspace creation timestamp.
  name: createdOn
  type: string
- description: Last modification timestamp.
  name: updatedOn
  type: string
- description: Aggregate statistics for the workspace.
  name: statistics
  type: object
provider_name: Intralinks
provider_slug: intralinks
schema_file: json-schema/workspace.json
slug: workspace
source_filename: workspace.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"workspace.json\",\n  \"title\": \"Intralinks Workspace\",\n  \"description\": \"A workspace (exchange or virtual data room) in the Intralinks platform used for secure document sharing and collaboration during M&A transactions, due diligence, and other confidential business processes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the workspace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workspace.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of workspace (e.g., ATC, ILP).\"\n    },\n    \"phase\": {\n      \"type\": \"string\",\n      \"description\": \"Current phase of the workspace lifecycle.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the workspace.\"\
  \n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Host organization name.\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Workspace creation timestamp.\"\n    },\n    \"updatedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp.\"\n    },\n    \"statistics\": {\n      \"type\": \"object\",\n      \"description\": \"Aggregate statistics for the workspace.\",\n      \"properties\": {\n        \"documentCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of documents.\"\n        },\n        \"folderCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of folders.\"\n        },\n        \"userCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of users.\"\n        },\n        \"groupCount\": {\n          \"type\"\
  : \"integer\",\n          \"description\": \"Total number of groups.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/json-schema/workspace.json
tags:
- Document Management
- Secure File Sharing
- Virtual Data Room
title: Intralinks Workspace
---
