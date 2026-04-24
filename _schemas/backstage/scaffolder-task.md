---
description: Task schema from Backstage scaffolder API
layout: schema
name: Task
properties_list:
- description: The unique identifier of the task.
  name: id
  type: string
- description: ''
  name: spec
  type: object
- description: The current status of the task.
  name: status
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: lastHeartbeatAt
  type: string
- description: ''
  name: completedAt
  type: string
- description: The user who created the task.
  name: createdBy
  type: string
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/scaffolder-task-schema.json
slug: scaffolder-task
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: Task
---
