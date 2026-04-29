---
description: ''
layout: schema
name: ActivityLogsMeta
properties_list:
- description: An array of activity logs sorted by timestamp in ascending order by default.
  name: activityLogs
  type: array
- description: Encodes the last event (the most recent event)
  name: cursor
  type: string
- description: Whether there is a next page of events
  name: nextPage
  type: boolean
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-activity-logs-activity-logs-meta-schema.json
slug: figma-activity-logs-activity-logs-meta
source_filename: figma-activity-logs-activity-logs-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActivityLogsMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activityLogs\": {\n      \"type\": \"array\",\n      \"description\": \"An array of activity logs sorted by timestamp in ascending order by default.\"\n    },\n    \"cursor\": {\n      \"type\": \"string\",\n      \"description\": \"Encodes the last event (the most recent event)\"\n    },\n    \"nextPage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether there is a next page of events\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-activity-logs-activity-logs-meta-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ActivityLogsMeta
---
