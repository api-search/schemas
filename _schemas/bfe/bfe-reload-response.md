---
description: Result of a configuration reload operation.
layout: schema
name: ReloadResponse
properties_list:
- description: Whether the reload succeeded.
  name: success
  type: boolean
- description: Human-readable result message.
  name: message
  type: string
- description: Name of the reloaded configuration.
  name: name
  type: string
provider_name: BFE
provider_slug: bfe
schema_file: json-schema/bfe-reload-response-schema.json
slug: bfe-reload-response
tags:
- Load Balancer
- Networking
- Open Source
- Traffic Management
- CNCF
- Baidu
title: ReloadResponse
---
