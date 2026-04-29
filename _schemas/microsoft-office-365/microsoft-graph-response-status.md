---
description: The response status of an attendee or organizer for a meeting request.
layout: schema
name: ResponseStatus
properties_list:
- description: The response type.
  name: response
  type: string
- description: The date and time the response was returned.
  name: time
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-response-status-schema.json
slug: microsoft-graph-response-status
source_filename: microsoft-graph-response-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseStatus\",\n  \"type\": \"object\",\n  \"description\": \"The response status of an attendee or organizer for a meeting request.\",\n  \"properties\": {\n    \"response\": {\n      \"type\": \"string\",\n      \"description\": \"The response type.\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the response was returned.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-response-status-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: ResponseStatus
---
