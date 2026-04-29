---
description: ReportSuiteList schema
layout: schema
name: ReportSuiteList
properties_list:
- description: ''
  name: content
  type: array
- description: ''
  name: totalElements
  type: integer
- description: ''
  name: totalPages
  type: integer
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/analytics-api-report-suite-list-schema.json
slug: analytics-api-report-suite-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-report-suite-list-schema.json\",\n  \"title\": \"ReportSuiteList\",\n  \"description\": \"ReportSuiteList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"rsid\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"currency\": {\n            \"type\": \"string\"\n          },\n          \"timezone\": {\n            \"type\": \"integer\"\n          },\n          \"calendarType\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"totalElements\": {\n      \"type\": \"integer\"\n    },\n    \"totalPages\": {\n      \"type\": \"\
  integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-report-suite-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: ReportSuiteList
---
