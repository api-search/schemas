---
description: Paginated list of audit events.
layout: schema
name: EventListResponse
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: meta
  type: object
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-event-list-response-schema.json
slug: bettercloud-event-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-event-list-response-schema.json\",\n  \"title\": \"EventListResponse\",\n  \"description\": \"Paginated list of audit events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Event\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/components/schemas/MetaResponse\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-event-list-response-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: EventListResponse
---
