---
description: Payload for ingesting a monitoring alert.
layout: schema
name: AlertRequest
properties_list:
- description: BigPanda application key for routing.
  name: app_key
  type: string
- description: Alert status.
  name: status
  type: string
- description: Hostname associated with the alert.
  name: host
  type: string
- description: Check or metric name that triggered the alert.
  name: check
  type: string
- description: Human-readable alert description.
  name: description
  type: string
- description: Unix timestamp of the alert.
  name: timestamp
  type: integer
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-alert-request-schema.json
slug: bigpanda-alert-request
tags:
- Incidents
- Monitoring
- Platform
title: AlertRequest
---
