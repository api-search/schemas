---
description: ''
layout: schema
name: ReportType
properties_list:
- description: The ID of the report type.
  name: id
  type: string
- description: The name of the report type.
  name: name
  type: string
- description: Whether the report type is system-managed.
  name: systemManaged
  type: boolean
- description: The date and time when the report type was deprecated.
  name: deprecateTime
  type: string
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-reporting-report-type-schema.json
slug: youtube-reporting-report-type
source_filename: youtube-reporting-report-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the report type.\",\n      \"example\": \"abc123def456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the report type.\",\n      \"example\": \"Example Title\"\n    },\n    \"systemManaged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the report type is system-managed.\",\n      \"example\": true\n    },\n    \"deprecateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the report type was deprecated.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportType\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-reporting-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-reporting-report-type-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: ReportType
---
