---
description: A People Task represents a human-in-the-loop task within an Appmixer flow that requires manual approval or action before the workflow can proceed.
layout: schema
name: Appmixer People Task
properties_list:
- description: Unique identifier for the task.
  name: id
  type: string
- description: The flow that generated this task.
  name: flowId
  type: string
- description: The role of the user in relation to this task.
  name: role
  type: string
- description: Current status of the task.
  name: status
  type: string
- description: Timestamp when the task was created.
  name: createdAt
  type: string
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/people-task.json
slug: people-task
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer People Task
---
