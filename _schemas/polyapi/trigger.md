---
description: A trigger connects a cloud event source (such as a webhook) to a function for event-driven execution.
layout: schema
name: PolyAPI Trigger
properties_list:
- description: The unique identifier of the trigger.
  name: id
  type: string
- description: The name of the trigger.
  name: name
  type: string
- description: A description of the trigger.
  name: description
  type: string
- description: The type of event source (e.g., webhook, cloud event).
  name: sourceType
  type: string
- description: The ID of the event source.
  name: sourceId
  type: string
- description: The ID of the function to trigger.
  name: targetFunctionId
  type: string
- description: The type of function to trigger.
  name: targetFunctionType
  type: string
- description: The state of the trigger.
  name: state
  type: string
- description: Timestamp when the trigger was created.
  name: createdAt
  type: string
- description: Timestamp when the trigger was last updated.
  name: updatedAt
  type: string
provider_name: PolyAPI
provider_slug: polyapi
schema_file: json-schema/trigger.json
slug: trigger
source_filename: trigger.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/polyapi/blob/main/json-schema/trigger.json\",\n  \"title\": \"PolyAPI Trigger\",\n  \"description\": \"A trigger connects a cloud event source (such as a webhook) to a function for event-driven execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the trigger.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the trigger.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the trigger.\"\n    },\n    \"sourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event source (e.g., webhook, cloud event).\"\n    },\n    \"sourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the event source.\"\n    },\n    \"targetFunctionId\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The ID of the function to trigger.\"\n    },\n    \"targetFunctionType\": {\n      \"type\": \"string\",\n      \"enum\": [\"server\", \"api\"],\n      \"description\": \"The type of function to trigger.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\"],\n      \"description\": \"The state of the trigger.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the trigger was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the trigger was last updated.\"\n    }\n  },\n  \"required\": [\"name\", \"sourceType\", \"sourceId\", \"targetFunctionId\", \"targetFunctionType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/json-schema/trigger.json
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
title: PolyAPI Trigger
---
