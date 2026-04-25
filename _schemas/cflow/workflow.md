---
description: A Workflow defines an automated business process with stages, rules, and field configurations in Cflow.
layout: schema
name: Cflow Workflow
properties_list:
- description: Unique identifier of the workflow.
  name: id
  type: string
- description: Name of the workflow.
  name: name
  type: string
- description: Description of the workflow.
  name: description
  type: string
- description: Current status of the workflow.
  name: status
  type: string
- description: List of process stages in the workflow.
  name: stages
  type: array
- description: Timestamp when the workflow was created.
  name: createdAt
  type: string
- description: Timestamp when the workflow was last updated.
  name: updatedAt
  type: string
provider_name: Cflow
provider_slug: cflow
schema_file: json-schema/workflow.json
slug: workflow
tags:
- Automations
- Business Process Automation
- Integrations
- No-Code
- Platform
- Protocols
- Rules
- Workflows
title: Cflow Workflow
---
