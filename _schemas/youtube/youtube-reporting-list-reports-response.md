---
description: ''
layout: schema
name: ListReportsResponse
properties_list:
- description: The list of reports.
  name: reports
  type: array
- description: A token to retrieve the next page of results.
  name: nextPageToken
  type: string
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-reporting-list-reports-response-schema.json
slug: youtube-reporting-list-reports-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"reports\": {\n      \"type\": \"array\",\n      \"description\": \"The list of reports.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The server-generated ID of the report.\",\n            \"example\": \"abc123def456\"\n          },\n          \"jobId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the job that created this report.\",\n            \"example\": \"abc123def456\"\n          },\n          \"startTime\": {\n            \"type\": \"string\",\n            \"description\": \"The start of the time period that the report covers.\",\n            \"example\": \"2026-01-15T10:30:00Z\",\n            \"format\": \"date-time\"\n          },\n          \"endTime\": {\n            \"type\": \"string\",\n            \"description\": \"The end of\
  \ the time period that the report covers.\",\n            \"example\": \"2026-01-15T10:30:00Z\",\n            \"format\": \"date-time\"\n          },\n          \"createTime\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time when the report was created.\",\n            \"example\": \"2026-01-15T10:30:00Z\",\n            \"format\": \"date-time\"\n          },\n          \"downloadUrl\": {\n            \"type\": \"string\",\n            \"description\": \"The URL from which the report can be downloaded.\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"jobExpireTime\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time when the job creating this report will expire.\",\n            \"example\": \"2026-01-15T10:30:00Z\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"A\
  \ token to retrieve the next page of results.\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListReportsResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-reporting-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-reporting-list-reports-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: ListReportsResponse
---
