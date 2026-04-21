---
description: Payload for ingesting a change event.
layout: schema
name: ChangeRequest
properties_list:
- description: Human-readable change summary.
  name: summary
  type: string
- description: Change status.
  name: status
  type: string
- description: Unique change identifier.
  name: identifier
  type: string
- description: Hosts affected by the change.
  name: hosts
  type: array
- description: Unix timestamp of the change.
  name: timestamp
  type: integer
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-change-request-schema.json
slug: bigpanda-change-request
tags:
- Incidents
- Monitoring
- Platform
title: ChangeRequest
---
