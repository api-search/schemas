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
source_filename: clockodo-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://my.clockodo.com/schemas/entry.json\",\n  \"title\": \"Clockodo Time Entry\",\n  \"description\": \"Schema for a Clockodo time-tracking entry. An entry records time spent by a user on a customer/project/service combination, optionally with billable status, hourly rate, and free-text description. Entries underpin reporting, invoicing, and project-budget tracking in Clockodo.\",\n  \"type\": \"object\",\n  \"required\": [\"customers_id\", \"services_id\", \"users_id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the entry.\"\n    },\n    \"users_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the user who recorded the entry.\"\n    },\n    \"customers_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the customer associated with the entry.\"\n    },\n    \"projects_id\": {\n   \
  \   \"type\": [\"integer\", \"null\"],\n      \"description\": \"ID of the project the entry is booked against.\"\n    },\n    \"services_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the service performed.\"\n    },\n    \"time_since\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the entry.\"\n    },\n    \"time_until\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"End time of the entry. Null when the entry is still being timed by the stop-clock.\"\n    },\n    \"duration\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Duration of the entry in seconds.\"\n    },\n    \"billable\": {\n      \"type\": \"integer\",\n      \"description\": \"0 = not billable, 1 = billable, 2 = already billed.\",\n      \"enum\": [0, 1, 2]\n    },\n    \"hourly_rate\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Effective\
  \ hourly rate (in account currency).\"\n    },\n    \"text\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Free-text description of the work performed.\"\n    },\n    \"lumpsum\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Lump-sum amount when the entry is billed as a flat fee instead of by time.\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/clockodo/refs/heads/main/json-schema/clockodo-entry-schema.json
tags:
- Absence Management
- Billing
- Project Management
- Stop Clock
- Time Tracking
- Timesheets
title: Clockodo Time Entry
---
