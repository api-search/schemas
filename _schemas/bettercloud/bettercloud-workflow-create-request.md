---
description: Request body for creating a workflow.
layout: schema
name: WorkflowCreateRequest
properties_list:
- description: Name of the workflow.
  name: name
  type: string
- description: Description of the workflow.
  name: description
  type: string
- description: Trigger type for the workflow.
  name: trigger_type
  type: string
- description: Initial status.
  name: status
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-workflow-create-request-schema.json
slug: bettercloud-workflow-create-request
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: WorkflowCreateRequest
---
