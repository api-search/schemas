---
description: Request body for triggering a custom workflow event
layout: schema
name: TriggerEventRequest
properties_list:
- description: Identifier of the user triggering the event
  name: userId
  type: string
- description: Event name to trigger
  name: event
  type: string
- description: Event payload data
  name: data
  type: object
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-trigger_event_request-schema.json
slug: alloy-embedded-trigger_event_request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-trigger_event_request-schema.json\",\n  \"title\": \"TriggerEventRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for triggering a custom workflow event\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user triggering the event\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"Event name to trigger\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Event payload data\"\n    }\n  },\n  \"required\": [\n    \"userId\",\n    \"event\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-trigger_event_request-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: TriggerEventRequest
---
