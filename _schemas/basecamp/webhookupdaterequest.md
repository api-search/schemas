---
description: ''
layout: schema
name: WebhookUpdateRequest
properties_list:
- description: Updated HTTPS URL for event delivery
  name: payload_url
  type: string
- description: Updated list of subscribed resource types
  name: types
  type: array
- description: Whether the webhook should be active
  name: active
  type: boolean
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/webhookupdaterequest-schema.json
slug: webhookupdaterequest
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: WebhookUpdateRequest
---
