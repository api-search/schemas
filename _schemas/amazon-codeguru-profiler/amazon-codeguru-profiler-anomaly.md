---
description: Details about an anomaly in a specific metric of application profile. The anomaly is detected using analysis of the metric data over a period of time.
layout: schema
name: Anomaly
properties_list:
- description: ''
  name: instances
  type: object
- description: ''
  name: metric
  type: object
- description: ''
  name: reason
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-anomaly-schema.json
slug: amazon-codeguru-profiler-anomaly
source_filename: amazon-codeguru-profiler-anomaly-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-anomaly-schema.json\",\n  \"title\": \"Anomaly\",\n  \"description\": \" Details about an anomaly in a specific metric of application profile. The anomaly is detected using analysis of the metric data over a period of time. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyInstances\"\n        },\n        {\n          \"description\": \" A list of the instances of the detected anomalies during the requested period. \"\n        }\n      ]\n    },\n    \"metric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Metric\"\n        },\n        {\n          \"description\": \" Details about the metric that the analysis used when it detected the\
  \ anomaly. The metric includes the name of the frame that was analyzed with the type and thread states used to derive the metric value for that frame. \"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason for which metric was flagged as anomalous.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"instances\",\n    \"metric\",\n    \"reason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-anomaly-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: Anomaly
---
