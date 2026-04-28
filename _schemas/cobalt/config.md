---
description: An integration configuration for a linked account within the Cobalt embedded integration platform.
layout: schema
name: Config
properties_list:
- description: Configuration ID.
  name: _id
  type: string
- description: Application slug.
  name: slug
  type: string
- description: The linked account ID.
  name: linked_account_id
  type: string
- description: Configuration fields.
  name: fields
  type: object
- description: Workflow enablement settings.
  name: workflows
  type: array
- description: Creation timestamp.
  name: created_at
  type: string
- description: Last update timestamp.
  name: updated_at
  type: string
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/config.json
slug: config
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Config
---
