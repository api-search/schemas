---
description: Payload for creating or updating an environment.
layout: schema
name: EnvironmentRequest
properties_list:
- description: Environment name.
  name: name
  type: string
- description: Environment description.
  name: description
  type: string
- description: Filter condition for grouping incidents.
  name: condition
  type: string
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-environment-request-schema.json
slug: bigpanda-environment-request
tags:
- Incidents
- Monitoring
- Platform
title: EnvironmentRequest
---
