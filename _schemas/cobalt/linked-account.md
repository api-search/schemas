---
description: A linked account representing an end-customer within the Cobalt embedded integration platform.
layout: schema
name: LinkedAccount
properties_list:
- description: Internal identifier.
  name: _id
  type: string
- description: The unique identifier for the linked account.
  name: linked_account_id
  type: string
- description: Display name.
  name: name
  type: string
- description: Custom metadata.
  name: your_app
  type: object
- description: Creation timestamp.
  name: created_at
  type: string
- description: Last update timestamp.
  name: updated_at
  type: string
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/linked-account.json
slug: linked-account
tags:
- Automation
- Embedded iPaaS
- Integrations
title: LinkedAccount
---
