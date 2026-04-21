---
description: A group from an integrated directory service.
layout: schema
name: Group
properties_list:
- description: Unique identifier for the group.
  name: id
  type: string
- description: Display name of the group.
  name: name
  type: string
- description: Email address of the group.
  name: email
  type: string
- description: Description of the group.
  name: description
  type: string
- description: Number of members in the group.
  name: member_count
  type: integer
- description: When the group was created.
  name: created_at
  type: string
- description: When the group was last updated.
  name: updated_at
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-group-schema.json
slug: bettercloud-group
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: Group
---
