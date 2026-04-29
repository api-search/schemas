---
description: Estimate of server calls for a proposed data repair job
layout: schema
name: ServerCallEstimate
properties_list:
- description: The report suite ID for the estimate
  name: reportSuiteId
  type: string
- description: Start date of the repair range
  name: dateRangeStart
  type: string
- description: End date of the repair range
  name: dateRangeEnd
  type: string
- description: Estimated number of server calls (rows) that will be scanned
  name: serverCallEstimate
  type: integer
- description: Token required when creating the repair job
  name: validationToken
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-data-repair-server-call-estimate-schema.json
slug: adobe-analytics-data-repair-server-call-estimate
source_filename: adobe-analytics-data-repair-server-call-estimate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Estimate of server calls for a proposed data repair job\",\n  \"properties\": {\n    \"reportSuiteId\": {\n      \"type\": \"string\",\n      \"description\": \"The report suite ID for the estimate\",\n      \"example\": \"500123\"\n    },\n    \"dateRangeStart\": {\n      \"type\": \"string\",\n      \"description\": \"Start date of the repair range\",\n      \"format\": \"date\",\n      \"example\": \"2026-01-15\"\n    },\n    \"dateRangeEnd\": {\n      \"type\": \"string\",\n      \"description\": \"End date of the repair range\",\n      \"format\": \"date\",\n      \"example\": \"2026-01-15\"\n    },\n    \"serverCallEstimate\": {\n      \"type\": \"integer\",\n      \"description\": \"Estimated number of server calls (rows) that will be scanned\",\n      \"example\": 10\n    },\n    \"validationToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token required when creating the repair job\",\n      \"example\"\
  : \"CAUQAA\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServerCallEstimate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-data-repair-server-call-estimate-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ServerCallEstimate
---
