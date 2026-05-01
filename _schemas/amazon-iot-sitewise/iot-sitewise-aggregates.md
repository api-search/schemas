---
description: Contains the (pre-calculated) aggregate values for an asset property.
layout: schema
name: Aggregates
properties_list:
- description: ''
  name: average
  type: object
- description: ''
  name: count
  type: object
- description: ''
  name: maximum
  type: object
- description: ''
  name: minimum
  type: object
- description: ''
  name: sum
  type: object
- description: ''
  name: standardDeviation
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-aggregates-schema.json
slug: iot-sitewise-aggregates
source_filename: iot-sitewise-aggregates-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-aggregates-schema.json\",\n  \"title\": \"Aggregates\",\n  \"description\": \"Contains the (pre-calculated) aggregate values for an asset property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"average\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedDoubleValue\"\n        },\n        {\n          \"description\": \"The average (mean) value of the time series over a time interval window.\"\n        }\n      ]\n    },\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedDoubleValue\"\n        },\n        {\n          \"description\": \"The count of data points in the time series over a time interval window.\"\n        }\n      ]\n    },\n    \"maximum\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/AggregatedDoubleValue\"\n        },\n        {\n          \"description\": \"The maximum value of the time series over a time interval window.\"\n        }\n      ]\n    },\n    \"minimum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedDoubleValue\"\n        },\n        {\n          \"description\": \"The minimum value of the time series over a time interval window.\"\n        }\n      ]\n    },\n    \"sum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedDoubleValue\"\n        },\n        {\n          \"description\": \"The sum of the time series over a time interval window.\"\n        }\n      ]\n    },\n    \"standardDeviation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedDoubleValue\"\n        },\n        {\n          \"description\": \"The standard deviation of the time series over a time interval window.\"\n    \
  \    }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-aggregates-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: Aggregates
---
