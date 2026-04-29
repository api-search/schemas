---
description: ''
layout: schema
name: ListReportTypesResponse
properties_list:
- description: The list of report types.
  name: reportTypes
  type: array
- description: A token to retrieve the next page of results.
  name: nextPageToken
  type: string
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-reporting-list-report-types-response-schema.json
slug: youtube-reporting-list-report-types-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportTypes\": {\n      \"type\": \"array\",\n      \"description\": \"The list of report types.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the report type.\",\n            \"example\": \"abc123def456\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the report type.\",\n            \"example\": \"Example Title\"\n          },\n          \"systemManaged\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the report type is system-managed.\",\n            \"example\": true\n          },\n          \"deprecateTime\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time when the report type was deprecated.\",\n            \"example\": \"\
  2026-01-15T10:30:00Z\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"A token to retrieve the next page of results.\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListReportTypesResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-reporting-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-reporting-list-report-types-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: ListReportTypesResponse
---
