---
description: ''
layout: schema
name: GetActivityLogsResponseBody
properties_list:
- description: The response status code.
  name: status
  type: number
- description: For successful requests, this value is always `false`.
  name: error
  type: boolean
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-activity-logs-get-activity-logs-response-body-schema.json
slug: figma-activity-logs-get-activity-logs-response-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetActivityLogsResponseBody\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"number\",\n      \"description\": \"The response status code.\"\n    },\n    \"error\": {\n      \"type\": \"boolean\",\n      \"description\": \"For successful requests, this value is always `false`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-activity-logs-get-activity-logs-response-body-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetActivityLogsResponseBody
---
