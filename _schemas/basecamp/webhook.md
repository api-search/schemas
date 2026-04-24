---
description: ''
layout: schema
name: Webhook
properties_list:
- description: Webhook ID
  name: id
  type: integer
- description: Whether this webhook is currently active
  name: active
  type: boolean
- description: Timestamp when the webhook was created
  name: created_at
  type: string
- description: Timestamp when the webhook was last updated
  name: updated_at
  type: string
- description: HTTPS URL where Basecamp sends event notifications
  name: payload_url
  type: string
- description: Resource types that trigger this webhook
  name: types
  type: array
- description: API URL for this webhook
  name: url
  type: string
- description: Web URL for this webhook configuration
  name: app_url
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/webhook-schema.json
slug: webhook
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Webhook
---
