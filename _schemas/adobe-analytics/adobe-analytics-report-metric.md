---
description: A metric included in a report request
layout: schema
name: ReportMetric
properties_list:
- description: The metric ID (e.g. metrics/visits)
  name: id
  type: string
- description: Column identifier for this metric in the response
  name: columnId
  type: string
- description: Metric-level filter IDs referencing metricFilters
  name: filters
  type: array
- description: Sort direction for this metric
  name: sort
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-report-metric-schema.json
slug: adobe-analytics-report-metric
source_filename: adobe-analytics-report-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A metric included in a report request\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The metric ID (e.g. metrics/visits)\",\n      \"example\": \"abc123\"\n    },\n    \"columnId\": {\n      \"type\": \"string\",\n      \"description\": \"Column identifier for this metric in the response\",\n      \"example\": \"500123\"\n    },\n    \"filters\": {\n      \"type\": \"array\",\n      \"description\": \"Metric-level filter IDs referencing metricFilters\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sort\": {\n      \"type\": \"string\",\n      \"description\": \"Sort direction for this metric\",\n      \"example\": \"ASC\",\n      \"enum\": [\n        \"ASC\",\n        \"DESC\"\n      ]\n    }\n  },\n  \"required\": [\n    \"id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportMetric\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-report-metric-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ReportMetric
---
