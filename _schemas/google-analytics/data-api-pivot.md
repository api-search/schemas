---
description: Describes the visible dimension columns and rows in the report response.
layout: schema
name: Pivot
properties_list:
- description: Dimension names for visible columns in the report response. Including "dateRange" produces a date range column; for each row in the response, dimension values in the date range column will indicate th
  name: fieldNames
  type: array
- description: The number of unique combinations of dimension values to return in this pivot. The `limit` parameter is required. A `limit` of 10,000 is common for single pivot requests. The product of the `limit` fo
  name: limit
  type: string
- description: Aggregate the metrics by dimensions in this pivot using the specified metric_aggregations.
  name: metricAggregations
  type: array
- description: The row count of the start row. The first row is counted as row 0.
  name: offset
  type: string
- description: Specifies how dimensions are ordered in the pivot. In the first Pivot, the OrderBys determine Row and PivotDimensionHeader ordering; in subsequent Pivots, the OrderBys determine only PivotDimensionHea
  name: orderBys
  type: array
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/data-api-pivot-schema.json
slug: data-api-pivot
source_filename: data-api-pivot-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-pivot-schema.json\",\n  \"title\": \"Pivot\",\n  \"description\": \"Describes the visible dimension columns and rows in the report response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldNames\": {\n      \"description\": \"Dimension names for visible columns in the report response. Including \\\"dateRange\\\" produces a date range column; for each row in the response, dimension values in the date range column will indicate the corresponding date range from the request.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"limit\": {\n      \"description\": \"The number of unique combinations of dimension values to return in this pivot. The `limit` parameter is required. A `limit` of 10,000 is common for single pivot requests.\
  \ The product of the `limit` for each `pivot` in a `RunPivotReportRequest` must not exceed 250,000. For example, a two pivot request with `limit: 1000` in each pivot will fail because the product is `1,000,000`.\",\n      \"format\": \"int64\",\n      \"type\": \"string\"\n    },\n    \"metricAggregations\": {\n      \"description\": \"Aggregate the metrics by dimensions in this pivot using the specified metric_aggregations.\",\n      \"items\": {\n        \"enum\": [\n          \"METRIC_AGGREGATION_UNSPECIFIED\",\n          \"TOTAL\",\n          \"MINIMUM\",\n          \"MAXIMUM\",\n          \"COUNT\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"offset\": {\n      \"description\": \"The row count of the start row. The first row is counted as row 0.\",\n      \"format\": \"int64\",\n      \"type\": \"string\"\n    },\n    \"orderBys\": {\n      \"description\": \"Specifies how dimensions are ordered in the pivot. In the first Pivot, the\
  \ OrderBys determine Row and PivotDimensionHeader ordering; in subsequent Pivots, the OrderBys determine only PivotDimensionHeader ordering. Dimensions specified in these OrderBys must be a subset of Pivot.field_names.\",\n      \"items\": {\n        \"description\": \"Order bys define how rows will be sorted in the response. For example, ordering rows by descending event count is one ordering, and ordering rows by the event name string is a different ordering.\",\n        \"properties\": {\n          \"desc\": {\n            \"description\": \"If true, sorts by descending order.\",\n            \"type\": \"boolean\"\n          },\n          \"dimension\": {\n            \"$ref\": \"#/components/schemas/DimensionOrderBy\",\n            \"description\": \"Sorts results by a dimension's values.\"\n          },\n          \"metric\": {\n            \"$ref\": \"#/components/schemas/MetricOrderBy\",\n            \"description\": \"Sorts results by a metric's values.\"\n          },\n      \
  \    \"pivot\": {\n            \"$ref\": \"#/components/schemas/PivotOrderBy\",\n            \"description\": \"Sorts results by a metric's values within a pivot column group.\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-pivot-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: Pivot
---
