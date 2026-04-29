---
description: An audit log event recording an action performed within an Airtable enterprise account. Events capture who performed what action, on which resource, and when, for compliance and security monitoring purposes.
layout: schema
name: Airtable Audit Log Event
properties_list:
- description: The unique identifier for the audit log event.
  name: id
  type: string
- description: The exact date and time when the action was logged, in ISO 8601 format.
  name: timestamp
  type: string
- description: The type of action that was performed (e.g., created, updated, deleted, viewed, shared).
  name: action
  type: string
- description: The entity that performed the action.
  name: actor
  type: object
- description: The ID of the model (base, table, field, record, view, etc.) that was affected by the action.
  name: modelId
  type:
  - string
  - 'null'
- description: The type of model affected by the action.
  name: modelType
  type:
  - string
  - 'null'
- description: The category of the event for organizational and filtering purposes.
  name: category
  type: string
- description: Additional context about the event, including related resource identifiers and request metadata.
  name: context
  type: object
- description: The version of the event payload format.
  name: payloadVersion
  type: string
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-audit-log-event-schema.json
slug: airtable-audit-log-event
source_filename: airtable-audit-log-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/audit-log-event.json\",\n  \"title\": \"Airtable Audit Log Event\",\n  \"description\": \"An audit log event recording an action performed within an Airtable enterprise account. Events capture who performed what action, on which resource, and when, for compliance and security monitoring purposes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the audit log event.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The exact date and time when the action was logged, in ISO 8601 format.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The type of action that was performed (e.g., created, updated, deleted, viewed, shared).\"\n    },\n    \"actor\": {\n      \"type\": \"\
  object\",\n      \"description\": \"The entity that performed the action.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of actor that initiated the action.\",\n          \"enum\": [\"user\", \"system\", \"anonymous\"]\n        },\n        \"userId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID of the user who performed the action. Null for system or anonymous actors.\"\n        },\n        \"email\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"email\",\n          \"description\": \"The email of the user who performed the action.\"\n        },\n        \"name\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The display name of the actor.\"\n        }\n      },\n      \"required\": [\"type\"]\n    },\n    \"modelId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the model (base, table,\
  \ field, record, view, etc.) that was affected by the action.\"\n    },\n    \"modelType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The type of model affected by the action.\",\n      \"enum\": [\"base\", \"table\", \"field\", \"record\", \"view\", \"workspace\", \"share\", \"user\", \"group\", \"interface\", null]\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the event for organizational and filtering purposes.\",\n      \"enum\": [\"app\", \"user\", \"share\", \"enterprise\", \"workspace\", \"interface\"]\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context about the event, including related resource identifiers and request metadata.\",\n      \"properties\": {\n        \"baseId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID of the base where the event occurred.\"\n        },\n        \"tableId\": {\n          \"type\"\
  : [\"string\", \"null\"],\n          \"description\": \"The ID of the table where the event occurred.\"\n        },\n        \"viewId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID of the view involved in the event.\"\n        },\n        \"workspaceId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID of the workspace where the event occurred.\"\n        },\n        \"interfaceId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID of the interface involved in the event.\"\n        },\n        \"actionId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A unique identifier for the specific action taken.\"\n        },\n        \"ipAddress\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The IP address from which the action was performed.\"\n        }\n      }\n    },\n    \"payloadVersion\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The version of the event payload format.\"\n    }\n  },\n  \"required\": [\"id\", \"timestamp\", \"action\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-audit-log-event-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable Audit Log Event
---
