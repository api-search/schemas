---
description: Represents an Engage flow in the Gong platform, which is an automated outreach sequence used for prospect engagement.
layout: schema
name: Gong Engage Flow
properties_list:
- description: Unique identifier for the flow.
  name: id
  type: string
- description: Name of the flow.
  name: name
  type: string
- description: Email of the flow owner.
  name: ownerEmail
  type: string
- description: ID of the folder containing the flow.
  name: folderId
  type: string
- description: Current status of the flow.
  name: status
  type: string
- description: Number of steps in the flow.
  name: stepsCount
  type: integer
- description: Number of prospects currently in the flow.
  name: prospectsCount
  type: integer
- description: The workspace the flow belongs to.
  name: workspaceId
  type: string
- description: When the flow was created.
  name: created
  type: string
- description: When the flow was last modified.
  name: modified
  type: string
provider_name: Gong
provider_slug: gong
schema_file: json-schema/gong-flow-schema.json
slug: gong-flow
source_filename: gong-flow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gong/blob/main/json-schema/gong-flow-schema.json\",\n  \"title\": \"Gong Engage Flow\",\n  \"description\": \"Represents an Engage flow in the Gong platform, which is an automated outreach sequence used for prospect engagement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the flow.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the flow.\"\n    },\n    \"ownerEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email of the flow owner.\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the folder containing the flow.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Paused\", \"Archived\", \"Draft\"],\n\
  \      \"description\": \"Current status of the flow.\"\n    },\n    \"stepsCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of steps in the flow.\"\n    },\n    \"prospectsCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of prospects currently in the flow.\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The workspace the flow belongs to.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the flow was created.\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the flow was last modified.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/json-schema/gong-flow-schema.json
tags: []
title: Gong Engage Flow
---
