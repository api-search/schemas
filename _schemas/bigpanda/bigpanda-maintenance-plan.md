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
source_filename: bigpanda-maintenance-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MaintenancePlan\",\n  \"type\": \"object\",\n  \"description\": \"A BigPanda maintenance plan for suppressing alerts.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Maintenance plan ID.\",\n      \"example\": \"mp-abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Maintenance plan name.\",\n      \"example\": \"Weekend Maintenance\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the maintenance plan is currently active.\",\n      \"example\": false\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Start Unix timestamp.\",\n      \"example\": 1713000000\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"description\": \"End Unix timestamp.\",\n      \"example\": 1713086400\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-maintenance-plan-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: MaintenancePlan
---
