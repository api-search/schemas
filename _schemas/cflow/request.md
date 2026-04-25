---
description: A Request is a submission within a workflow that moves through stages for review, approval, or rejection.
layout: schema
name: Cflow Request
properties_list:
- description: Unique identifier of the request.
  name: id
  type: string
- description: Identifier of the associated workflow.
  name: workflowId
  type: string
- description: Current status of the request.
  name: status
  type: string
- description: Name or identifier of the current process stage.
  name: currentStage
  type: string
- description: Dynamic key-value pairs representing the form field data for the request.
  name: fields
  type: object
- description: Username of the person who submitted the request.
  name: submittedBy
  type: string
- description: Timestamp when the request was created.
  name: createdAt
  type: string
- description: Timestamp when the request was last updated.
  name: updatedAt
  type: string
provider_name: Cflow
provider_slug: cflow
schema_file: json-schema/request.json
slug: request
tags:
- Automations
- Business Process Automation
- Integrations
- No-Code
- Platform
- Protocols
- Rules
- Workflows
title: Cflow Request
---
