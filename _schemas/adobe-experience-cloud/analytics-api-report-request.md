---
description: ReportRequest schema
layout: schema
name: ReportRequest
properties_list:
- description: Report suite ID.
  name: rsid
  type: string
- description: ''
  name: globalFilters
  type: array
- description: ''
  name: metricContainer
  type: object
- description: ''
  name: dimension
  type: string
- description: ''
  name: settings
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/analytics-api-report-request-schema.json
slug: analytics-api-report-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-report-request-schema.json\",\n  \"title\": \"ReportRequest\",\n  \"description\": \"ReportRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rsid\": {\n      \"type\": \"string\",\n      \"description\": \"Report suite ID.\"\n    },\n    \"globalFilters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"dateRange\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"metricContainer\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"metrics\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n  \
  \            \"id\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"dimension\": {\n      \"type\": \"string\"\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"limit\": {\n          \"type\": \"integer\"\n        },\n        \"page\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-report-request-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: ReportRequest
---
