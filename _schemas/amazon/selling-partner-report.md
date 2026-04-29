---
description: Report schema from Amazon Selling Partner API
layout: schema
name: Report
properties_list:
- description: ''
  name: reportId
  type: string
- description: ''
  name: reportType
  type: string
- description: ''
  name: processingStatus
  type: string
- description: ''
  name: reportDocumentId
  type: string
- description: ''
  name: createdTime
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-report-schema.json
slug: selling-partner-report
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportId\": {\n      \"type\": \"string\"\n    },\n    \"reportType\": {\n      \"type\": \"string\"\n    },\n    \"processingStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CANCELLED\",\n        \"DONE\",\n        \"FATAL\",\n        \"IN_PROGRESS\",\n        \"IN_QUEUE\"\n      ]\n    },\n    \"reportDocumentId\": {\n      \"type\": \"string\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Report\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-report-schema.json\",\n  \"description\": \"Report schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-report-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: Report
---
