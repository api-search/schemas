---
description: A Stage represents a step in a workflow process where requests are reviewed, approved, or routed.
layout: schema
name: Cflow Stage
properties_list:
- description: Unique identifier of the stage.
  name: id
  type: string
- description: Name of the process stage.
  name: name
  type: string
- description: Order of the stage in the workflow.
  name: order
  type: integer
- description: Users assigned as reviewers for this stage.
  name: reviewers
  type: array
provider_name: Cflow
provider_slug: cflow
schema_file: json-schema/stage.json
slug: stage
tags:
- Automations
- Business Process Automation
- Integrations
- No-Code
- Platform
- Protocols
- Rules
- Workflows
title: Cflow Stage
---
