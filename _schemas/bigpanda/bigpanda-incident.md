---
description: A correlated incident from multiple alerts.
layout: schema
name: Incident
properties_list:
- description: Incident ID.
  name: id
  type: string
- description: Incident status.
  name: status
  type: string
- description: Incident severity level.
  name: severity
  type: string
- description: Incident description.
  name: description
  type: string
- description: Number of correlated alerts.
  name: alerts_count
  type: integer
- description: Unix timestamp when incident started.
  name: started_at
  type: integer
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-incident-schema.json
slug: bigpanda-incident
tags:
- Incidents
- Monitoring
- Platform
title: Incident
---
