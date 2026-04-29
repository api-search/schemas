---
description: An event object representing a change to a resource, delivered asynchronously to the target location of an active webhook subscription.
layout: schema
name: Asana Webhook Event
properties_list:
- description: The user who triggered the event. May be null for system-generated events.
  name: user
  type: object
- description: The resource that triggered the event by being modified.
  name: resource
  type: object
- description: Deprecated. The type of the resource that generated the event.
  name: type
  type: string
- description: The type of action taken on the resource.
  name: action
  type: string
- description: For added/removed events, the parent object. Null for other event types.
  name: parent
  type: object
- description: The timestamp when the event occurred.
  name: created_at
  type: string
- description: Information about the field-level change. Only present when action is 'changed'.
  name: change
  type:
  - object
  - 'null'
provider_name: Asana
provider_slug: asana
schema_file: json-schema/asana-webhook-event-json-schema.json
slug: asana-webhook-event-json
source_filename: asana-webhook-event-json-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developers.asana.com/schemas/webhook-event\",\n  \"title\": \"Asana Webhook Event\",\n  \"description\": \"An event object representing a change to a resource, delivered asynchronously to the target location of an active webhook subscription.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/UserCompact\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The user who triggered the event. May be null for system-generated events.\"\n    },\n    \"resource\": {\n      \"$ref\": \"#/$defs/AsanaNamedResource\",\n      \"description\": \"The resource that triggered the event by being modified.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Deprecated. The type of the resource that generated the event.\",\n      \"examples\": [\"task\"]\n    },\n    \"action\": {\n      \"\
  type\": \"string\",\n      \"enum\": [\"changed\", \"added\", \"removed\", \"deleted\", \"undeleted\"],\n      \"description\": \"The type of action taken on the resource.\",\n      \"examples\": [\"changed\"]\n    },\n    \"parent\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/AsanaNamedResource\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"For added/removed events, the parent object. Null for other event types.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the event occurred.\",\n      \"examples\": [\"2024-01-15T10:30:00.000Z\"]\n    },\n    \"change\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Information about the field-level change. Only present when action is 'changed'.\",\n      \"properties\": {\n        \"field\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the field that has changed.\",\n\
  \          \"examples\": [\"assignee\"]\n        },\n        \"action\": {\n          \"type\": \"string\",\n          \"enum\": [\"changed\", \"added\", \"removed\"],\n          \"description\": \"The type of action taken on the field.\",\n          \"examples\": [\"changed\"]\n        },\n        \"new_value\": {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"The new value when change.action is 'changed' and value is an Asana resource.\",\n          \"properties\": {\n            \"gid\": { \"type\": \"string\" },\n            \"resource_type\": { \"type\": \"string\" }\n          }\n        },\n        \"added_value\": {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"The added value when change.action is 'added' and value is an Asana resource.\",\n          \"properties\": {\n            \"gid\": { \"type\": \"string\" },\n            \"resource_type\": { \"type\": \"string\" }\n          }\n        },\n        \"removed_value\"\
  : {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"The removed value when change.action is 'removed' and value is an Asana resource.\",\n          \"properties\": {\n            \"gid\": { \"type\": \"string\" },\n            \"resource_type\": { \"type\": \"string\" }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"resource\", \"action\", \"created_at\"],\n  \"$defs\": {\n    \"UserCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\", \"const\": \"user\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"AsanaNamedResource\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/asana/refs/heads/main/json-schema/asana-webhook-event-json-schema.json
tags:
- Collaboration
- Productivity
- Project Management
- Projects
- Task Management
- Tasks
- Workflow
title: Asana Webhook Event
---
