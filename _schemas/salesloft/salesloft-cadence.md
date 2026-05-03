---
description: A Cadence in Salesloft is a structured sequence of touchpoints (calls, emails, tasks) designed to engage prospects.
layout: schema
name: Salesloft Cadence
properties_list:
- description: Unique identifier for the cadence
  name: id
  type: integer
- description: Name of the cadence
  name: name
  type: string
- description: Description of the cadence purpose
  name: description
  type: string
- description: Current state of the cadence
  name: current_state
  type: string
- description: Functional purpose of the cadence (e.g. outbound, inbound, event)
  name: cadence_function
  type: string
- description: Whether this is a team cadence (shared) vs personal
  name: is_team
  type: boolean
- description: Whether the cadence is shared across the team
  name: shared
  type: boolean
- description: ID of the user who owns this cadence
  name: owner_id
  type: integer
- description: Whether this cadence is a team-level cadence
  name: team_cadence
  type: boolean
- description: Whether to remove people with bounced emails
  name: remove_bounced
  type: boolean
- description: Whether opt-out links are included in emails
  name: opt_out_link_included
  type: boolean
- description: Whether this cadence is still in draft state
  name: draft
  type: boolean
- description: Timestamp when cadence was archived
  name: archived_at
  type: string
- description: Timestamp when the cadence was created
  name: created_at
  type: string
- description: Timestamp when the cadence was last updated
  name: updated_at
  type: string
provider_name: Salesloft
provider_slug: salesloft
schema_file: json-schema/salesloft-cadence-schema.json
slug: salesloft-cadence
source_filename: salesloft-cadence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/salesloft/json-schema/salesloft-cadence-schema.json\",\n  \"title\": \"Salesloft Cadence\",\n  \"description\": \"A Cadence in Salesloft is a structured sequence of touchpoints (calls, emails, tasks) designed to engage prospects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the cadence\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the cadence\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the cadence purpose\"\n    },\n    \"current_state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the cadence\",\n      \"enum\": [\"draft\", \"active\", \"archived\"]\n    },\n    \"cadence_function\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Functional purpose of the cadence (e.g. outbound, inbound, event)\"\n    },\n    \"is_team\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a team cadence (shared) vs personal\"\n    },\n    \"shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cadence is shared across the team\"\n    },\n    \"owner_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the user who owns this cadence\"\n    },\n    \"team_cadence\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this cadence is a team-level cadence\"\n    },\n    \"remove_bounced\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to remove people with bounced emails\"\n    },\n    \"opt_out_link_included\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether opt-out links are included in emails\"\n    },\n    \"draft\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this cadence is still in draft\
  \ state\"\n    },\n    \"archived_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when cadence was archived\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the cadence was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the cadence was last updated\"\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesloft/refs/heads/main/json-schema/salesloft-cadence-schema.json
tags:
- Sales
- CRM
- Revenue
- Automation
- AI
title: Salesloft Cadence
---
