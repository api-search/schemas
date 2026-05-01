---
description: The structure representing the BatchGetFrameMetricDataRequest.
layout: schema
name: BatchGetFrameMetricDataRequest
properties_list:
- description: ''
  name: frameMetrics
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-batch-get-frame-metric-data-request-schema.json
slug: amazon-codeguru-profiler-batch-get-frame-metric-data-request
source_filename: amazon-codeguru-profiler-batch-get-frame-metric-data-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-batch-get-frame-metric-data-request-schema.json\",\n  \"title\": \"BatchGetFrameMetricDataRequest\",\n  \"description\": \"The structure representing the BatchGetFrameMetricDataRequest.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"frameMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameMetrics\"\n        },\n        {\n          \"description\": \" The details of the metrics that are used to request a time series of values. The metric includes the name of the frame, the aggregation type to calculate the metric value for the frame, and the thread states to use to get the count for the metric value of the frame.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-batch-get-frame-metric-data-request-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: BatchGetFrameMetricDataRequest
---
