---
description: An Adobe Analytics report suite
layout: schema
name: ReportSuite
properties_list:
- description: Report suite ID
  name: rsid
  type: string
- description: Display name of the report suite
  name: name
  type: string
- description: Timezone for the report suite
  name: timezoneZoneinfo
  type: string
- description: Report suite type
  name: type
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-report-suite-schema.json
slug: adobe-analytics-report-suite
source_filename: adobe-analytics-report-suite-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An Adobe Analytics report suite\",\n  \"properties\": {\n    \"rsid\": {\n      \"type\": \"string\",\n      \"description\": \"Report suite ID\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the report suite\",\n      \"example\": \"Example Title\"\n    },\n    \"timezoneZoneinfo\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone for the report suite\",\n      \"example\": \"example_value\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Report suite type\",\n      \"example\": \"standard\",\n      \"enum\": [\n        \"standard\",\n        \"virtual\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportSuite\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-report-suite-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ReportSuite
---
