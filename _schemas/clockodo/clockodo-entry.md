---
description: Schema for a Clockodo time-tracking entry. An entry records time spent by a user on a customer/project/service combination, optionally with billable status, hourly rate, and free-text description. Entries underpin reporting, invoicing, and project-budget tracking in Clockodo.
layout: schema
name: Clockodo Time Entry
properties_list:
- description: Unique identifier of the entry.
  name: id
  type: integer
- description: ID of the user who recorded the entry.
  name: users_id
  type: integer
- description: ID of the customer associated with the entry.
  name: customers_id
  type: integer
- description: ID of the project the entry is booked against.
  name: projects_id
  type:
  - integer
  - 'null'
- description: ID of the service performed.
  name: services_id
  type: integer
- description: Start time of the entry.
  name: time_since
  type: string
- description: End time of the entry. Null when the entry is still being timed by the stop-clock.
  name: time_until
  type:
  - string
  - 'null'
- description: Duration of the entry in seconds.
  name: duration
  type:
  - integer
  - 'null'
- description: 0 = not billable, 1 = billable, 2 = already billed.
  name: billable
  type: integer
- description: Effective hourly rate (in account currency).
  name: hourly_rate
  type:
  - number
  - 'null'
- description: Free-text description of the work performed.
  name: text
  type:
  - string
  - 'null'
- description: Lump-sum amount when the entry is billed as a flat fee instead of by time.
  name: lumpsum
  type:
  - number
  - 'null'
provider_name: Clockodo
provider_slug: clockodo
schema_file: json-schema/clockodo-entry-schema.json
slug: clockodo-entry
tags:
- Absence Management
- Billing
- Project Management
- Stop Clock
- Time Tracking
- Timesheets
title: Clockodo Time Entry
---
