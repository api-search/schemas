---
description: Payload for creating a maintenance plan.
layout: schema
name: MaintenancePlanRequest
properties_list:
- description: Maintenance plan name.
  name: name
  type: string
- description: Filter condition for hosts in maintenance.
  name: condition
  type: string
- description: Start Unix timestamp.
  name: start
  type: integer
- description: End Unix timestamp.
  name: end
  type: integer
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-maintenance-plan-request-schema.json
slug: bigpanda-maintenance-plan-request
tags:
- Incidents
- Monitoring
- Platform
title: MaintenancePlanRequest
---
