---
description: The payload delivered by ClickUp when a webhook event is triggered. Each payload includes the event type, webhook identifier, and an array of history items describing the specific changes that occurred.
layout: schema
name: ClickUp Webhook Payload
properties_list:
- description: The name of the event that triggered the webhook.
  name: event
  type: string
- description: The unique identifier of the webhook subscription that matched this event.
  name: webhook_id
  type: string
- description: The ID of the task involved in the event. Present for task-related events.
  name: task_id
  type: string
- description: The ID of the list involved in the event. Present for list-related events.
  name: list_id
  type: string
- description: The ID of the folder involved in the event. Present for folder-related events.
  name: folder_id
  type: string
- description: The ID of the space involved in the event. Present for space-related events.
  name: space_id
  type: string
- description: The ID of the goal involved in the event. Present for goal and key result events.
  name: goal_id
  type: string
- description: Array of change records describing what was modified in this event.
  name: history_items
  type: array
provider_name: clickup
provider_slug: clickup
schema_file: json-schema/clickup-webhook-payload-schema.json
slug: clickup-webhook-payload
source_filename: clickup-webhook-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.clickup.com/schemas/clickup/webhook-payload.json\",\n  \"title\": \"ClickUp Webhook Payload\",\n  \"description\": \"The payload delivered by ClickUp when a webhook event is triggered. Each payload includes the event type, webhook identifier, and an array of history items describing the specific changes that occurred.\",\n  \"type\": \"object\",\n  \"required\": [\"event\", \"webhook_id\"],\n  \"properties\": {\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event that triggered the webhook.\",\n      \"enum\": [\n        \"taskCreated\",\n        \"taskUpdated\",\n        \"taskDeleted\",\n        \"taskPriorityUpdated\",\n        \"taskStatusUpdated\",\n        \"taskAssigneeUpdated\",\n        \"taskDueDateUpdated\",\n        \"taskTagUpdated\",\n        \"taskMoved\",\n        \"taskCommentPosted\",\n        \"taskCommentUpdated\"\
  ,\n        \"taskTimeEstimateUpdated\",\n        \"taskTimeTrackedUpdated\",\n        \"listCreated\",\n        \"listUpdated\",\n        \"listDeleted\",\n        \"folderCreated\",\n        \"folderUpdated\",\n        \"folderDeleted\",\n        \"spaceCreated\",\n        \"spaceUpdated\",\n        \"spaceDeleted\",\n        \"goalCreated\",\n        \"goalUpdated\",\n        \"goalDeleted\",\n        \"keyResultCreated\",\n        \"keyResultUpdated\",\n        \"keyResultDeleted\"\n      ]\n    },\n    \"webhook_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the webhook subscription that matched this event.\"\n    },\n    \"task_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the task involved in the event. Present for task-related events.\"\n    },\n    \"list_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the list involved in the event. Present for list-related events.\"\n    },\n    \"folder_id\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The ID of the folder involved in the event. Present for folder-related events.\"\n    },\n    \"space_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the space involved in the event. Present for space-related events.\"\n    },\n    \"goal_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the goal involved in the event. Present for goal and key result events.\"\n    },\n    \"history_items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/HistoryItem\"\n      },\n      \"description\": \"Array of change records describing what was modified in this event.\"\n    }\n  },\n  \"$defs\": {\n    \"HistoryItem\": {\n      \"type\": \"object\",\n      \"description\": \"A single change record within a webhook event payload.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the\
  \ history item.\"\n        },\n        \"type\": {\n          \"type\": \"integer\",\n          \"description\": \"The type code of the history item.\"\n        },\n        \"date\": {\n          \"type\": \"string\",\n          \"description\": \"Unix timestamp in milliseconds when the change occurred.\",\n          \"pattern\": \"^[0-9]+$\"\n        },\n        \"field\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the field that was changed (e.g., status, priority, assignee, due_date, tag, comment, name, description, time_estimate, time_spent).\"\n        },\n        \"parent_id\": {\n          \"type\": \"string\",\n          \"description\": \"The parent resource ID.\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"description\": \"Additional contextual data about the change.\"\n        },\n        \"source\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The source of the change. Null\
  \ for changes made through the UI, 'api' for API changes.\"\n        },\n        \"user\": {\n          \"$ref\": \"#/$defs/WebhookUser\"\n        },\n        \"before\": {\n          \"description\": \"The value of the field before the change. Type varies based on the field.\"\n        },\n        \"after\": {\n          \"description\": \"The value of the field after the change. Type varies based on the field.\"\n        }\n      },\n      \"required\": [\"id\", \"date\", \"field\", \"user\"]\n    },\n    \"WebhookUser\": {\n      \"type\": \"object\",\n      \"description\": \"The user who performed the action that triggered the webhook event.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the user.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user.\"\n        },\n        \"email\": {\n          \"type\": \"string\"\
  ,\n          \"format\": \"email\",\n          \"description\": \"The email address of the user.\"\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"The hex color code associated with the user.\"\n        },\n        \"profilePicture\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL of the user's profile picture.\"\n        },\n        \"initials\": {\n          \"type\": \"string\",\n          \"description\": \"The initials of the user.\",\n          \"maxLength\": 3\n        }\n      },\n      \"required\": [\"id\", \"username\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/json-schema/clickup-webhook-payload-schema.json
tags: []
title: ClickUp Webhook Payload
---
