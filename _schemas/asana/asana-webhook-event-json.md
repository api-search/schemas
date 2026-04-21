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
