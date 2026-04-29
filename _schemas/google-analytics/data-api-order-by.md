---
description: Order bys define how rows will be sorted in the response. For example, ordering rows by descending event count is one ordering, and ordering rows by the event name string is a different ordering.
layout: schema
name: OrderBy
properties_list:
- description: If true, sorts by descending order.
  name: desc
  type: boolean
- description: Sorts by dimension values.
  name: dimension
  type: object
- description: Sorts by metric values.
  name: metric
  type: object
- description: Sorts by a pivot column group.
  name: pivot
  type: object
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/data-api-order-by-schema.json
slug: data-api-order-by
source_filename: data-api-order-by-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-order-by-schema.json\",\n  \"title\": \"OrderBy\",\n  \"description\": \"Order bys define how rows will be sorted in the response. For example, ordering rows by descending event count is one ordering, and ordering rows by the event name string is a different ordering.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"desc\": {\n      \"description\": \"If true, sorts by descending order.\",\n      \"type\": \"boolean\"\n    },\n    \"dimension\": {\n      \"description\": \"Sorts by dimension values.\",\n      \"properties\": {\n        \"dimensionName\": {\n          \"description\": \"A dimension name in the request to order by.\",\n          \"type\": \"string\",\n          \"example\": \"Example Name\"\n        },\n        \"orderType\": {\n          \"description\": \"Controls the\
  \ rule for dimension value ordering.\",\n          \"enum\": [\n            \"ORDER_TYPE_UNSPECIFIED\",\n            \"ALPHANUMERIC\",\n            \"CASE_INSENSITIVE_ALPHANUMERIC\",\n            \"NUMERIC\"\n          ],\n          \"type\": \"string\",\n          \"example\": \"ORDER_TYPE_UNSPECIFIED\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"metric\": {\n      \"description\": \"Sorts by metric values.\",\n      \"properties\": {\n        \"metricName\": {\n          \"description\": \"A metric name in the request to order by.\",\n          \"type\": \"string\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"pivot\": {\n      \"description\": \"Sorts by a pivot column group.\",\n      \"properties\": {\n        \"metricName\": {\n          \"description\": \"In the response to order by, order rows by this column. Must be a metric name from the request.\",\n          \"type\": \"string\"\n        },\n        \"pivotSelections\": {\n          \"\
  description\": \"Used to select a dimension name and value pivot. If multiple pivot selections are given, the sort occurs on rows where all pivot selection dimension name and value pairs match the row's dimension name and value pair.\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/PivotSelection\"\n          },\n          \"type\": \"array\"\n        }\n      },\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-order-by-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: OrderBy
---
