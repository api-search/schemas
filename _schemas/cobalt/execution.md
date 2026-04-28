---
description: A workflow execution record within the Cobalt embedded integration platform.
layout: schema
name: Execution
properties_list:
- description: Execution ID.
  name: _id
  type: string
- description: The workflow that was executed.
  name: workflow_id
  type: string
- description: The linked account ID.
  name: linked_account_id
  type: string
- description: Execution status.
  name: status
  type: string
- description: Execution start timestamp.
  name: started_at
  type: string
- description: Execution completion timestamp.
  name: completed_at
  type: string
- description: Execution logs.
  name: logs
  type: array
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/execution.json
slug: execution
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Execution
---
