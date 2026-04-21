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
tags: []
title: ClickUp Webhook Payload
---
