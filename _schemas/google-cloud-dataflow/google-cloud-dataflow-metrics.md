---
description: Contains metrics and their values for a Dataflow job, including counters, distributions, and other execution metrics that provide insight into pipeline performance.
layout: schema
name: Google Cloud Dataflow Job Metrics
properties_list:
- description: Timestamp as of which metric values are current.
  name: metricTime
  type: string
- description: All metrics for this job.
  name: metrics
  type: array
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
schema_file: json-schema/google-cloud-dataflow-metrics-schema.json
slug: google-cloud-dataflow-metrics
source_filename: google-cloud-dataflow-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/google-cloud-dataflow/json-schema/google-cloud-dataflow-metrics-schema.json\",\n  \"title\": \"Google Cloud Dataflow Job Metrics\",\n  \"description\": \"Contains metrics and their values for a Dataflow job, including counters, distributions, and other execution metrics that provide insight into pipeline performance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp as of which metric values are current.\"\n    },\n    \"metrics\": {\n      \"type\": \"array\",\n      \"description\": \"All metrics for this job.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MetricUpdate\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"MetricUpdate\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the state of a metric at a particular point\
  \ in time.\",\n      \"properties\": {\n        \"name\": {\n          \"$ref\": \"#/$defs/MetricStructuredName\",\n          \"description\": \"The structured name of the metric.\"\n        },\n        \"kind\": {\n          \"type\": \"string\",\n          \"description\": \"Metric aggregation kind. Possible values include Sum, Max, Min, Mean, Set, And, Or, Distribution, LatestValue.\"\n        },\n        \"cumulative\": {\n          \"type\": \"boolean\",\n          \"description\": \"True if this metric is reported as the total cumulative aggregate value.\"\n        },\n        \"scalar\": {\n          \"description\": \"Worker-computed aggregate value for aggregation kinds Sum, Max, Min.\"\n        },\n        \"meanSum\": {\n          \"description\": \"Worker-computed aggregate sum value for the Mean aggregation kind.\"\n        },\n        \"meanCount\": {\n          \"description\": \"Worker-computed aggregate count value for the Mean aggregation kind.\"\n        },\n       \
  \ \"set\": {\n          \"description\": \"Worker-computed aggregate value for the Set aggregation kind.\"\n        },\n        \"distribution\": {\n          \"description\": \"A struct value describing properties of a distribution of numeric values.\"\n        },\n        \"gauge\": {\n          \"description\": \"A struct value describing properties of a gauge metric.\"\n        },\n        \"internal\": {\n          \"description\": \"Worker-computed aggregate value for internal use by the service.\"\n        },\n        \"updateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp associated with the metric value.\"\n        }\n      }\n    },\n    \"MetricStructuredName\": {\n      \"type\": \"object\",\n      \"description\": \"Identifies a metric, using both the key and the context in which it appears.\",\n      \"properties\": {\n        \"origin\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Origin (namespace) of metric name. Typical values are dataflow/v1b3 and user.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Worker-defined metric name.\"\n        },\n        \"context\": {\n          \"type\": \"object\",\n          \"description\": \"Zero or more labeled fields identifying the part of the job this metric is associated with.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/json-schema/google-cloud-dataflow-metrics-schema.json
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
title: Google Cloud Dataflow Job Metrics
---
