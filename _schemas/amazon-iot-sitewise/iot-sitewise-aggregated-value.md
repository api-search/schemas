---
description: Contains aggregated asset property values (for example, average, minimum, and maximum).
layout: schema
name: AggregatedValue
properties_list:
- description: ''
  name: timestamp
  type: object
- description: ''
  name: quality
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-aggregated-value-schema.json
slug: iot-sitewise-aggregated-value
source_filename: iot-sitewise-aggregated-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-aggregated-value-schema.json\",\n  \"title\": \"AggregatedValue\",\n  \"description\": \"Contains aggregated asset property values (for example, average, minimum, and maximum).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the aggregating computations occurred, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"quality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Quality\"\n        },\n        {\n          \"description\": \"The quality of the aggregated data.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Aggregates\"\
  \n        },\n        {\n          \"description\": \"The value of the aggregates.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"timestamp\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-aggregated-value-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AggregatedValue
---
