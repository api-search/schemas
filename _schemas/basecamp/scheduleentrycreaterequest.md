---
description: ''
layout: schema
name: ScheduleEntryCreateRequest
properties_list:
- description: Entry title/summary
  name: summary
  type: string
- description: Entry start time in ISO 8601 format
  name: starts_at
  type: string
- description: Entry end time in ISO 8601 format
  name: ends_at
  type: string
- description: HTML-formatted entry description
  name: description
  type: string
- description: Person IDs to add as participants
  name: participant_ids
  type: array
- description: Whether this is an all-day event
  name: all_day
  type: boolean
- description: Whether to notify participants
  name: notify
  type: boolean
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/scheduleentrycreaterequest-schema.json
slug: scheduleentrycreaterequest
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ScheduleEntryCreateRequest
---
