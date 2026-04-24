---
description: Represents the JSON payload delivered by Basecamp to a registered webhook endpoint when a subscribed event occurs within a project. Every payload includes a unique event ID, the event kind, a timestamp, the full recording object that triggered the event, the person who triggered it, and optional event-specific details.
layout: schema
name: Basecamp Webhook Payload
properties_list:
- description: Unique identifier for this webhook event delivery
  name: id
  type: integer
- description: Event type descriptor identifying the resource type and action, formatted as {resource}_{action} (e.g., message_created, todo_completed, comment_updated)
  name: kind
  type: string
- description: ISO 8601 UTC timestamp when the triggering event occurred in Basecamp
  name: created_at
  type: string
- description: Full JSON representation of the Basecamp resource that triggered the event
  name: recording
  type: object
- description: The Basecamp user whose action triggered the event
  name: creator
  type: object
- description: Event-specific contextual metadata. For copy and move events includes a copy object with the duplicated item reference. Contents vary by event kind.
  name: details
  type: object
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/basecamp-webhook-payload-schema.json
slug: basecamp-webhook-payload
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Basecamp Webhook Payload
---
