---
description: The frame name, metric type, and thread states. These are used to derive the value of the metric for the frame.
layout: schema
name: FrameMetric
properties_list:
- description: ''
  name: frameName
  type: object
- description: ''
  name: threadStates
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-frame-metric-schema.json
slug: amazon-codeguru-profiler-frame-metric
source_filename: amazon-codeguru-profiler-frame-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-frame-metric-schema.json\",\n  \"title\": \"FrameMetric\",\n  \"description\": \" The frame name, metric type, and thread states. These are used to derive the value of the metric for the frame.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"frameName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" Name of the method common across the multiple occurrences of a frame in an application profile.\"\n        }\n      ]\n    },\n    \"threadStates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThreadStates\"\n        },\n        {\n          \"description\": \"List of application runtime thread states used to get the counts for a frame a derive\
  \ a metric value.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricType\"\n        },\n        {\n          \"description\": \" A type of aggregation that specifies how a metric for a frame is analyzed. The supported value <code>AggregatedRelativeTotalTime</code> is an aggregation of the metric value for one frame that is calculated across the occurrences of all frames in a profile. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"frameName\",\n    \"threadStates\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-frame-metric-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: FrameMetric
---
