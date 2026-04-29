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
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MaintenancePlanRequest\",\n  \"type\": \"object\",\n  \"description\": \"Payload for creating a maintenance plan.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Maintenance plan name.\",\n      \"example\": \"Weekend Maintenance\"\n    },\n    \"condition\": {\n      \"type\": \"string\",\n      \"description\": \"Filter condition for hosts in maintenance.\",\n      \"example\": \"host = \\\"production-database-1\\\"\"\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Start Unix timestamp.\",\n      \"example\": 1713000000\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"description\": \"End Unix timestamp.\",\n      \"example\": 1713086400\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"condition\",\n    \"start\",\n    \"end\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-maintenance-plan-request-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: MaintenancePlanRequest
---
