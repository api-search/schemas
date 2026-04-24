---
description: A configured webhook for Vendr event notifications
layout: schema
name: Webhook
properties_list:
- description: Unique webhook identifier
  name: id
  type: string
- description: Webhook endpoint URL
  name: url
  type: string
- description: Subscribed event types
  name: events
  type: array
- description: Whether the webhook is active
  name: active
  type: boolean
provider_name: Blissfully
provider_slug: blissfully
schema_file: json-schema/blissfully-webhook-schema.json
slug: blissfully-webhook
tags:
- Procurement
- SaaS Discovery
- SaaS Management
- Software Procurement
- Spend Optimization
- Vendor Management
title: Webhook
---
