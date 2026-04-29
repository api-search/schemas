---
description: A filter applied to a report
layout: schema
name: ReportFilter
properties_list:
- description: Filter type
  name: type
  type: string
- description: ISO 8601 date range (e.g. 2024-01-01T00:00:00/2024-01-31T23:59:59)
  name: dateRange
  type: string
- description: ID of an existing segment to apply as a filter
  name: segmentId
  type: string
- description: Dimension for breakdown filter
  name: dimension
  type: string
- description: Dimension item ID for breakdown filter
  name: itemId
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-report-filter-schema.json
slug: adobe-analytics-report-filter
source_filename: adobe-analytics-report-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A filter applied to a report\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Filter type\",\n      \"example\": \"dateRange\",\n      \"enum\": [\n        \"dateRange\",\n        \"breakdown\",\n        \"segment\"\n      ]\n    },\n    \"dateRange\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 date range (e.g. 2024-01-01T00:00:00/2024-01-31T23:59:59)\",\n      \"example\": \"example_value\"\n    },\n    \"segmentId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of an existing segment to apply as a filter\",\n      \"example\": \"500123\"\n    },\n    \"dimension\": {\n      \"type\": \"string\",\n      \"description\": \"Dimension for breakdown filter\",\n      \"example\": \"example_value\"\n    },\n    \"itemId\": {\n      \"type\": \"string\",\n      \"description\": \"Dimension item ID for breakdown filter\",\n      \"example\": \"500123\"\
  \n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportFilter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-report-filter-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ReportFilter
---
