---
description: Contains a timestamp with optional nanosecond granularity.
layout: schema
name: TimeInNanos
properties_list:
- description: ''
  name: timeInSeconds
  type: object
- description: ''
  name: offsetInNanos
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-time-in-nanos-schema.json
slug: iot-sitewise-time-in-nanos
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-time-in-nanos-schema.json\",\n  \"title\": \"TimeInNanos\",\n  \"description\": \"Contains a timestamp with optional nanosecond granularity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timeInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeInSeconds\"\n        },\n        {\n          \"description\": \"The timestamp date, in seconds, in the Unix epoch format. Fractional nanosecond data is provided by <code>offsetInNanos</code>.\"\n        }\n      ]\n    },\n    \"offsetInNanos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OffsetInNanos\"\n        },\n        {\n          \"description\": \"The nanosecond offset from <code>timeInSeconds</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"timeInSeconds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-time-in-nanos-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: TimeInNanos
---
