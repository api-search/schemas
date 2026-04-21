---
description: A User represents an authenticated account in the Appmixer platform with access to flows, files, data stores, and connected third-party accounts.
layout: schema
name: Appmixer User
properties_list:
- description: Unique identifier for the user.
  name: id
  type: string
- description: The user's username, typically an email address.
  name: username
  type: string
- description: The user's email address.
  name: email
  type: string
- description: Authentication token for the user session.
  name: token
  type: string
- description: The subscription plan associated with the user.
  name: plan
  type: string
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/user.json
slug: user
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer User
---
