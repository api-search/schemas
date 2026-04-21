---
description: A BigPanda maintenance plan for suppressing alerts.
layout: schema
name: MaintenancePlan
properties_list:
- description: Maintenance plan ID.
  name: id
  type: string
- description: Maintenance plan name.
  name: name
  type: string
- description: Whether the maintenance plan is currently active.
  name: active
  type: boolean
- description: Start Unix timestamp.
  name: start
  type: integer
- description: End Unix timestamp.
  name: end
  type: integer
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-maintenance-plan-schema.json
slug: bigpanda-maintenance-plan
tags:
- Incidents
- Monitoring
- Platform
title: MaintenancePlan
---
