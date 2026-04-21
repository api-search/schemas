---
description: A single audit log entry.
layout: schema
name: AuditLogEntry
properties_list:
- description: Log entry ID.
  name: id
  type: string
- description: User who performed the action.
  name: user
  type: string
- description: Action performed.
  name: action
  type: string
- description: Unix timestamp.
  name: timestamp
  type: integer
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-audit-log-entry-schema.json
slug: bigpanda-audit-log-entry
tags:
- Incidents
- Monitoring
- Platform
title: AuditLogEntry
---
