---
description: A BigPanda environment for incident grouping.
layout: schema
name: Environment
properties_list:
- description: Environment ID.
  name: id
  type: string
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
schema_file: json-schema/bigpanda-environment-schema.json
slug: bigpanda-environment
tags:
- Incidents
- Monitoring
- Platform
title: Environment
---
