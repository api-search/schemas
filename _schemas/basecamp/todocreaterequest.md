---
description: ''
layout: schema
name: TodoCreateRequest
properties_list:
- description: To-do text description
  name: content
  type: string
- description: Additional details in HTML format
  name: description
  type: string
- description: Person IDs to assign to this to-do
  name: assignee_ids
  type: array
- description: Person IDs to notify when this to-do is completed
  name: completion_subscriber_ids
  type: array
- description: Whether to immediately notify assignees
  name: notify
  type: boolean
- description: Due date in ISO 8601 format
  name: due_on
  type: string
- description: Start date in ISO 8601 format
  name: starts_on
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/todocreaterequest-schema.json
slug: todocreaterequest
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: TodoCreateRequest
---
