---
description: Paginated list of report suites
layout: schema
name: ReportSuiteList
properties_list:
- description: ''
  name: content
  type: array
- description: Total number of report suites
  name: totalElements
  type: integer
- description: Total number of pages
  name: totalPages
  type: integer
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-report-suite-list-schema.json
slug: adobe-analytics-report-suite-list
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Paginated list of report suites\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An Adobe Analytics report suite\",\n        \"properties\": {\n          \"rsid\": {\n            \"type\": \"string\",\n            \"description\": \"Report suite ID\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name of the report suite\",\n            \"example\": \"Example Title\"\n          },\n          \"timezoneZoneinfo\": {\n            \"type\": \"string\",\n            \"description\": \"Timezone for the report suite\",\n            \"example\": \"example_value\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Report suite type\",\n            \"example\"\
  : \"standard\",\n            \"enum\": [\n              \"standard\",\n              \"virtual\"\n            ]\n          }\n        }\n      }\n    },\n    \"totalElements\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of report suites\",\n      \"example\": 42\n    },\n    \"totalPages\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of pages\",\n      \"example\": 42\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportSuiteList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-report-suite-list-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ReportSuiteList
---
