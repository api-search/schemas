---
description: Response after ingesting a change event.
layout: schema
name: ChangeResponse
properties_list:
- description: Internal change ID.
  name: _id
  type: string
- description: Ingestion status.
  name: status
  type: string
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-change-response-schema.json
slug: bigpanda-change-response
tags:
- Incidents
- Monitoring
- Platform
title: ChangeResponse
---
