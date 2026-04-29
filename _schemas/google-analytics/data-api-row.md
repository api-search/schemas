---
description: 'Report data for each row. For example if RunReportRequest contains: ```none "dimensions": [ { "name": "eventName" }, { "name": "countryId" } ], "metrics": [ { "name": "eventCount" } ] ``` One row with ''in_app_purchase'' as the eventName, ''JP'' as the countryId, and 15 as the eventCount, would be: ```none "dimensionValues": [ { "value": "in_app_purchase" }, { "value": "JP" } ], "metricValues": [ { "value": "15" } ] ```'
layout: schema
name: Row
properties_list:
- description: List of requested dimension values. In a PivotReport, dimension_values are only listed for dimensions included in a pivot.
  name: dimensionValues
  type: array
- description: List of requested visible metric values.
  name: metricValues
  type: array
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/data-api-row-schema.json
slug: data-api-row
source_filename: data-api-row-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-row-schema.json\",\n  \"title\": \"Row\",\n  \"description\": \"Report data for each row. For example if RunReportRequest contains: ```none \\\"dimensions\\\": [ { \\\"name\\\": \\\"eventName\\\" }, { \\\"name\\\": \\\"countryId\\\" } ], \\\"metrics\\\": [ { \\\"name\\\": \\\"eventCount\\\" } ] ``` One row with 'in_app_purchase' as the eventName, 'JP' as the countryId, and 15 as the eventCount, would be: ```none \\\"dimensionValues\\\": [ { \\\"value\\\": \\\"in_app_purchase\\\" }, { \\\"value\\\": \\\"JP\\\" } ], \\\"metricValues\\\": [ { \\\"value\\\": \\\"15\\\" } ] ```\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dimensionValues\": {\n      \"description\": \"List of requested dimension values. In a PivotReport, dimension_values are only listed for dimensions included in a pivot.\"\
  ,\n      \"items\": {\n        \"description\": \"The value of a dimension.\",\n        \"properties\": {\n          \"value\": {\n            \"description\": \"Value as a string if the dimension type is a string.\",\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"metricValues\": {\n      \"description\": \"List of requested visible metric values.\",\n      \"items\": {\n        \"description\": \"The value of a metric.\",\n        \"properties\": {\n          \"value\": {\n            \"description\": \"Measurement value. See MetricHeader for type.\",\n            \"type\": \"string\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-row-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: Row
---
