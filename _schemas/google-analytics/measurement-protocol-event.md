---
description: Event schema from Google Analytics API
layout: schema
name: Event
properties_list:
- description: The name of the event. Must not use reserved names (ad_click, app_exception, error, session_start, etc.) or reserved prefixes (_, firebase_, ga_, google_, gtag.).
  name: name
  type: string
- description: Event parameters as key-value pairs. Common parameters include session_id, engagement_time_msec, and timestamp_micros.
  name: params
  type: object
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/measurement-protocol-event-schema.json
slug: measurement-protocol-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-event-schema.json\",\n  \"title\": \"Event\",\n  \"description\": \"Event schema from Google Analytics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event. Must not use reserved names (ad_click, app_exception, error, session_start, etc.) or reserved prefixes (_, firebase_, ga_, google_, gtag.).\",\n      \"example\": \"Example Name\"\n    },\n    \"params\": {\n      \"type\": \"object\",\n      \"description\": \"Event parameters as key-value pairs. Common parameters include session_id, engagement_time_msec, and timestamp_micros.\",\n      \"additionalProperties\": true,\n      \"properties\": {\n        \"session_id\": {\n          \"type\": \"string\",\n          \"description\": \"Session\
  \ identifier for accurate session metrics.\"\n        },\n        \"engagement_time_msec\": {\n          \"type\": \"integer\",\n          \"description\": \"User engagement duration in milliseconds.\"\n        },\n        \"timestamp_micros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Unix epoch time in microseconds to override event timestamp.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-event-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: Event
---
