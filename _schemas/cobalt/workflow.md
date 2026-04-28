---
description: A public workflow within the Cobalt embedded integration platform.
layout: schema
name: Workflow
properties_list:
- description: Workflow ID.
  name: _id
  type: string
- description: Workflow name.
  name: name
  type: string
- description: Workflow description.
  name: description
  type: string
- description: Workflow nodes.
  name: nodes
  type: array
- description: Creation timestamp.
  name: created_at
  type: string
- description: Last update timestamp.
  name: updated_at
  type: string
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/workflow.json
slug: workflow
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Workflow
---
