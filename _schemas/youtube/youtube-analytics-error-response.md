---
description: A standard error response returned by the YouTube Analytics API.
layout: schema
name: ErrorResponse
properties_list:
- description: The error details.
  name: error
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-analytics-error-response-schema.json
slug: youtube-analytics-error-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A standard error response returned by the YouTube Analytics API.\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"The error details.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"integer\",\n          \"description\": \"The HTTP status code of the error.\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable description of the error.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The error status code.\"\n        },\n        \"details\": {\n          \"type\": \"array\",\n          \"description\": \"A list of additional error details.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n       \
  \         \"description\": \"The type of the error detail.\"\n              },\n              \"reason\": {\n                \"type\": \"string\",\n                \"description\": \"The reason code for the error.\"\n              },\n              \"domain\": {\n                \"type\": \"string\",\n                \"description\": \"The domain in which the error occurred.\"\n              },\n              \"metadata\": {\n                \"type\": \"object\",\n                \"description\": \"Additional metadata about the error.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-analytics-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-analytics-error-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: ErrorResponse
---
