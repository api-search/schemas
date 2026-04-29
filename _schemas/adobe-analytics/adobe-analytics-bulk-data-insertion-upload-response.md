---
description: Response after a successful file upload
layout: schema
name: UploadResponse
properties_list:
- description: Unique tracking code for this upload
  name: uploadTrackingCode
  type: string
- description: Size of the uploaded file in bytes
  name: fileSize
  type: integer
- description: Timestamp when the file was received
  name: receivedTime
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-bulk-data-insertion-upload-response-schema.json
slug: adobe-analytics-bulk-data-insertion-upload-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response after a successful file upload\",\n  \"properties\": {\n    \"uploadTrackingCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique tracking code for this upload\",\n      \"example\": \"example_value\"\n    },\n    \"fileSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the uploaded file in bytes\",\n      \"example\": 10\n    },\n    \"receivedTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the file was received\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UploadResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-bulk-data-insertion-upload-response-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: UploadResponse
---
