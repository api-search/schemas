---
description: ReportStatus schema from Amazon Advertising API
layout: schema
name: ReportStatus
properties_list:
- description: ''
  name: reportId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: fileSize
  type: integer
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/advertising-report-status-schema.json
slug: advertising-report-status
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IN_PROGRESS\",\n        \"SUCCESS\",\n        \"FAILURE\"\n      ]\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"fileSize\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportStatus\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-report-status-schema.json\",\n  \"description\": \"ReportStatus schema from Amazon Advertising API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-report-status-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: ReportStatus
---
