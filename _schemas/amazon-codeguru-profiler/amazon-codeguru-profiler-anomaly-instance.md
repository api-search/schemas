---
description: The specific duration in which the metric is flagged as anomalous.
layout: schema
name: AnomalyInstance
properties_list:
- description: ''
  name: endTime
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: userFeedback
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-anomaly-instance-schema.json
slug: amazon-codeguru-profiler-anomaly-instance
source_filename: amazon-codeguru-profiler-anomaly-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-anomaly-instance-schema.json\",\n  \"title\": \"AnomalyInstance\",\n  \"description\": \"The specific duration in which the metric is flagged as anomalous.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The end time of the period during which the metric is flagged as anomalous. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The universally\
  \ unique identifier (UUID) of an instance of an anomaly in a metric. \"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The start time of the period during which the metric is flagged as anomalous. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \"\n        }\n      ]\n    },\n    \"userFeedback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserFeedback\"\n        },\n        {\n          \"description\": \"Feedback type on a specific instance of anomaly submitted by the user.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"startTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-anomaly-instance-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: AnomalyInstance
---
