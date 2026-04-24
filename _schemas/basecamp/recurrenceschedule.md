---
description: Recurrence configuration for a schedule entry
layout: schema
name: RecurrenceSchedule
properties_list:
- description: Recurrence frequency
  name: frequency
  type: string
- description: Days of the week for weekly recurrence
  name: days
  type: array
- description: Hour of the day for the recurrence
  name: hour
  type: integer
- description: Minute of the hour for the recurrence
  name: minute
  type: integer
- description: Week instance within the month for monthly recurrence
  name: week_instance
  type: integer
- description: Date when the recurrence starts
  name: start_date
  type: string
- description: Date when the recurrence ends
  name: end_date
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/recurrenceschedule-schema.json
slug: recurrenceschedule
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: RecurrenceSchedule
---
