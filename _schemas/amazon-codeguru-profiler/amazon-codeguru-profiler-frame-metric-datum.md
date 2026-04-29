---
description: Information about a frame metric and its values.
layout: schema
name: FrameMetricDatum
properties_list:
- description: ''
  name: frameMetric
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-frame-metric-datum-schema.json
slug: amazon-codeguru-profiler-frame-metric-datum
source_filename: amazon-codeguru-profiler-frame-metric-datum-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-frame-metric-datum-schema.json\",\n  \"title\": \"FrameMetricDatum\",\n  \"description\": \" Information about a frame metric and its values. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"frameMetric\": {\n      \"$ref\": \"#/components/schemas/FrameMetric\"\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameMetricValues\"\n        },\n        {\n          \"description\": \" A list of values that are associated with a frame metric. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"frameMetric\",\n    \"values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-frame-metric-datum-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: FrameMetricDatum
---
