---
description: A user discovered and managed across BetterCloud integrations.
layout: schema
name: User
properties_list:
- description: Unique identifier for the user in BetterCloud.
  name: id
  type: string
- description: Primary email address of the user.
  name: email
  type: string
- description: User's first name.
  name: first_name
  type: string
- description: User's last name.
  name: last_name
  type: string
- description: Current status of the user.
  name: status
  type: string
- description: Department or organizational unit.
  name: department
  type: string
- description: Job title.
  name: title
  type: string
- description: Email of the user's manager.
  name: manager_email
  type: string
- description: Office location.
  name: location
  type: string
- description: When the user was first discovered.
  name: created_at
  type: string
- description: When the user record was last updated.
  name: updated_at
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-user-schema.json
slug: bettercloud-user
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: User
---
