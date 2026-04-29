---
description: Details about the metric that the analysis used when it detected the anomaly. The metric what is analyzed to create recommendations. It includes the name of the frame that was analyzed and the type and thread states used to derive the metric value for that frame.
layout: schema
name: Metric
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
schema_file: json-schema/amazon-codeguru-profiler-metric-schema.json
slug: amazon-codeguru-profiler-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-metric-schema.json\",\n  \"title\": \"Metric\",\n  \"description\": \" Details about the metric that the analysis used when it detected the anomaly. The metric what is analyzed to create recommendations. It includes the name of the frame that was analyzed and the type and thread states used to derive the metric value for that frame. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"frameName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The name of the method that appears as a frame in any stack in a profile. \"\n        }\n      ]\n    },\n    \"threadStates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Strings\"\n        },\n     \
  \   {\n          \"description\": \" The list of application runtime thread states that is used to calculate the metric value for the frame. \"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricType\"\n        },\n        {\n          \"description\": \" A type that specifies how a metric for a frame is analyzed. The supported value <code>AggregatedRelativeTotalTime</code> is an aggregation of the metric value for one frame that is calculated across the occurences of all frames in a profile.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"frameName\",\n    \"threadStates\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-metric-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: Metric
---
