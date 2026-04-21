---
description: An audit event recording activity in BetterCloud or connected SaaS applications.
layout: schema
name: Event
properties_list:
- description: Unique identifier of the event.
  name: id
  type: string
- description: Event type in dot-notation (e.g., user.suspended, group.created).
  name: type
  type: string
- description: Email of the user or system that triggered the event.
  name: actor_email
  type: string
- description: Email of the user or resource affected by the event.
  name: target_email
  type: string
- description: Human-readable description of what happened.
  name: description
  type: string
- description: When the event occurred.
  name: occurred_at
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-event-schema.json
slug: bettercloud-event
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: Event
---
