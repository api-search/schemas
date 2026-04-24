---
description: A Boltic automation workflow consisting of triggers, nodes, and execution configuration for orchestrating tasks across integrations.
layout: schema
name: Boltic Workflow
properties_list:
- description: Unique identifier for the workflow
  name: id
  type: string
- description: Human-readable name for the workflow
  name: name
  type: string
- description: Description of what the workflow does
  name: description
  type: string
- description: Current status of the workflow
  name: status
  type: string
- description: ''
  name: trigger
  type: object
- description: Ordered list of action nodes in the workflow
  name: nodes
  type: array
- description: Tags for categorizing the workflow
  name: tags
  type: array
- description: Total number of times this workflow has been executed
  name: executionCount
  type: integer
- description: Timestamp of the last execution
  name: lastExecutedAt
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Boltic
provider_slug: boltic
schema_file: json-schema/boltic-workflow.json
slug: boltic-workflow
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
title: Boltic Workflow
---
