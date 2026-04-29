---
description: Container defining the metrics to include in a report
layout: schema
name: MetricContainer
properties_list:
- description: ''
  name: metrics
  type: array
- description: Filters applied at the metric level
  name: metricFilters
  type: array
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-metric-container-schema.json
slug: adobe-analytics-metric-container
source_filename: adobe-analytics-metric-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Container defining the metrics to include in a report\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A metric included in a report request\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The metric ID (e.g. metrics/visits)\",\n            \"example\": \"abc123\"\n          },\n          \"columnId\": {\n            \"type\": \"string\",\n            \"description\": \"Column identifier for this metric in the response\",\n            \"example\": \"500123\"\n          },\n          \"filters\": {\n            \"type\": \"array\",\n            \"description\": \"Metric-level filter IDs referencing metricFilters\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n\
  \          \"sort\": {\n            \"type\": \"string\",\n            \"description\": \"Sort direction for this metric\",\n            \"example\": \"ASC\",\n            \"enum\": [\n              \"ASC\",\n              \"DESC\"\n            ]\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      }\n    },\n    \"metricFilters\": {\n      \"type\": \"array\",\n      \"description\": \"Filters applied at the metric level\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A filter applied to a report\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Filter type\",\n            \"example\": \"dateRange\",\n            \"enum\": [\n              \"dateRange\",\n              \"breakdown\",\n              \"segment\"\n            ]\n          },\n          \"dateRange\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"ISO 8601 date range (e.g. 2024-01-01T00:00:00/2024-01-31T23:59:59)\",\n            \"example\": \"example_value\"\n          },\n          \"segmentId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of an existing segment to apply as a filter\",\n            \"example\": \"500123\"\n          },\n          \"dimension\": {\n            \"type\": \"string\",\n            \"description\": \"Dimension for breakdown filter\",\n            \"example\": \"example_value\"\n          },\n          \"itemId\": {\n            \"type\": \"string\",\n            \"description\": \"Dimension item ID for breakdown filter\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"type\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"metrics\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricContainer\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-metric-container-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: MetricContainer
---
