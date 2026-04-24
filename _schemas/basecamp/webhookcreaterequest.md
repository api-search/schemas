---
description: ''
layout: schema
name: WebhookCreateRequest
properties_list:
- description: HTTPS URL to receive webhook event notifications
  name: payload_url
  type: string
- description: Resource types to subscribe to. Omit to subscribe to all types.
  name: types
  type: array
- description: Whether the webhook should be active upon creation
  name: active
  type: boolean
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/webhookcreaterequest-schema.json
slug: webhookcreaterequest
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: WebhookCreateRequest
---
