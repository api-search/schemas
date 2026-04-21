---
description: An Account represents an authenticated connection to a third-party service (e.g. OAuth credentials for Slack, Google, etc.) belonging to an Appmixer user.
layout: schema
name: Appmixer Account
properties_list:
- description: Unique identifier for the connected account.
  name: accountId
  type: string
- description: Display name for the connected account.
  name: name
  type: string
- description: The service or connector this account is associated with (e.g. appmixer.google).
  name: service
  type: string
- description: Profile information retrieved from the third-party service.
  name: profileInfo
  type: object
- description: Whether the account credentials (tokens) are still valid.
  name: valid
  type: boolean
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/account.json
slug: account
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer Account
---
