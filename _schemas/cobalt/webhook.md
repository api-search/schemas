---
description: A webhook subscription for receiving real-time notifications when events occur in Cobalt.
layout: schema
name: Webhook
properties_list:
- description: Webhook ID.
  name: _id
  type: string
- description: The webhook notification URL.
  name: webhook_url
  type: string
- description: Subscribed event names.
  name: webhook_events
  type: array
- description: The linked account ID.
  name: linked_account_id
  type: string
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/webhook.json
slug: webhook
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Webhook
---
