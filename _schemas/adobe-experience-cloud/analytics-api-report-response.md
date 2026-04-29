---
description: ReportResponse schema
layout: schema
name: ReportResponse
properties_list:
- description: ''
  name: totalPages
  type: integer
- description: ''
  name: firstPage
  type: boolean
- description: ''
  name: lastPage
  type: boolean
- description: ''
  name: numberOfElements
  type: integer
- description: ''
  name: totalElements
  type: integer
- description: ''
  name: rows
  type: array
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/analytics-api-report-response-schema.json
slug: analytics-api-report-response
source_filename: analytics-api-report-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-report-response-schema.json\",\n  \"title\": \"ReportResponse\",\n  \"description\": \"ReportResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalPages\": {\n      \"type\": \"integer\"\n    },\n    \"firstPage\": {\n      \"type\": \"boolean\"\n    },\n    \"lastPage\": {\n      \"type\": \"boolean\"\n    },\n    \"numberOfElements\": {\n      \"type\": \"integer\"\n    },\n    \"totalElements\": {\n      \"type\": \"integer\"\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"itemId\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          },\n          \"data\": {\n            \"type\": \"array\",\n \
  \           \"items\": {\n              \"type\": \"number\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-report-response-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: ReportResponse
---
