---
description: An automation workflow that can be triggered to execute actions across SaaS applications.
layout: schema
name: Workflow
properties_list:
- description: Unique identifier of the workflow.
  name: id
  type: string
- description: Display name of the workflow.
  name: name
  type: string
- description: Description of what the workflow does.
  name: description
  type: string
- description: Current status of the workflow.
  name: status
  type: string
- description: How the workflow is triggered.
  name: trigger_type
  type: string
- description: Number of actions in the workflow.
  name: action_count
  type: integer
- description: When the workflow was created.
  name: created_at
  type: string
- description: When the workflow was last updated.
  name: updated_at
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-workflow-schema.json
slug: bettercloud-workflow
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: Workflow
---
