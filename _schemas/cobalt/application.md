---
description: An enabled application within the Cobalt embedded integration platform.
layout: schema
name: Application
properties_list:
- description: Application name.
  name: name
  type: string
- description: Application slug identifier.
  name: slug
  type: string
- description: Application icon URL.
  name: icon
  type: string
- description: Application description.
  name: description
  type: string
- description: Authentication type (e.g., oauth2, api_key).
  name: auth_type
  type: string
- description: Whether the application is connected for the linked account.
  name: connected
  type: boolean
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/application.json
slug: application
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Application
---
