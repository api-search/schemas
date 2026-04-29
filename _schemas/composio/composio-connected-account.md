---
description: Represents an authenticated connection between an end user and a third-party application, managed through Composio's OAuth flow.
layout: schema
name: Composio Connected Account
properties_list:
- description: Unique identifier for the connected account.
  name: id
  type: string
- description: The toolkit (application) this account is connected to.
  name: toolkit
  type: string
- description: Current status of the connection.
  name: status
  type: string
- description: Identifier for the end user entity that owns this connection.
  name: entityId
  type: string
- description: The auth configuration used for this connection.
  name: authConfigId
  type: string
- description: Timestamp when the connected account was created.
  name: createdAt
  type: string
provider_name: Composio
provider_slug: composio
schema_file: json-schema/composio-connected-account-schema.json
slug: composio-connected-account
source_filename: composio-connected-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://composio.dev/schemas/composio/connected-account.json\",\n  \"title\": \"Composio Connected Account\",\n  \"description\": \"Represents an authenticated connection between an end user and a third-party application, managed through Composio's OAuth flow.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"toolkit\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the connected account.\",\n      \"minLength\": 1\n    },\n    \"toolkit\": {\n      \"type\": \"string\",\n      \"description\": \"The toolkit (application) this account is connected to.\",\n      \"minLength\": 1\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the connection.\",\n      \"enum\": [\"active\", \"expired\", \"pending\"]\n    },\n    \"entityId\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"Identifier for the end user entity that owns this connection.\"\n    },\n    \"authConfigId\": {\n      \"type\": \"string\",\n      \"description\": \"The auth configuration used for this connection.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the connected account was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/composio/refs/heads/main/json-schema/composio-connected-account-schema.json
tags:
- AI Agents
- Authentication
- Integrations
- OAuth
- Tools
- Unified_API
title: Composio Connected Account
---
