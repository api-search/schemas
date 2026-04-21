---
description: A Flow represents an automation workflow in Appmixer, consisting of connected components that define integration logic between services.
layout: schema
name: Appmixer Flow
properties_list:
- description: Unique identifier for the flow.
  name: id
  type: string
- description: Human-readable name of the flow.
  name: name
  type: string
- description: Flow definition object containing the workflow graph and component configurations.
  name: flow
  type: object
- description: Current execution state of the flow.
  name: stage
  type: string
- description: Creation timestamp of the flow.
  name: btime
  type: string
- description: Last modification timestamp of the flow.
  name: mtime
  type: string
- description: URL or data URI of the flow thumbnail image.
  name: thumbnail
  type: string
- description: Custom metadata key-value pairs associated with the flow.
  name: customFields
  type: object
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/flow.json
slug: flow
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer Flow
---
