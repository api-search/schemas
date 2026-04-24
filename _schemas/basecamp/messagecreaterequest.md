---
description: ''
layout: schema
name: MessageCreateRequest
properties_list:
- description: Message subject (title)
  name: subject
  type: string
- description: Message body in HTML format
  name: content
  type: string
- description: Set to "active" to publish immediately
  name: status
  type: string
- description: Optional message category ID
  name: category_id
  type: integer
- description: Person IDs to notify about this message
  name: subscriptions
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/messagecreaterequest-schema.json
slug: messagecreaterequest
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: MessageCreateRequest
---
