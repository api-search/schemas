---
description: The structure representing the BatchGetFrameMetricDataResponse.
layout: schema
name: BatchGetFrameMetricDataResponse
properties_list:
- description: ''
  name: endTime
  type: object
- description: ''
  name: endTimes
  type: object
- description: ''
  name: frameMetricData
  type: object
- description: ''
  name: resolution
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: unprocessedEndTimes
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-batch-get-frame-metric-data-response-schema.json
slug: amazon-codeguru-profiler-batch-get-frame-metric-data-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-batch-get-frame-metric-data-response-schema.json\",\n  \"title\": \"BatchGetFrameMetricDataResponse\",\n  \"description\": \"The structure representing the BatchGetFrameMetricDataResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The end time of the time period for the returned time series values. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \"\n        }\n      ]\n    },\n    \"endTimes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfTimestamps\"\n        },\n        {\n\
  \          \"description\": \" List of instances, or time steps, in the time series. For example, if the <code>period</code> is one day (<code>PT24H)</code>), and the <code>resolution</code> is five minutes (<code>PT5M</code>), then there are 288 <code>endTimes</code> in the list that are each five minutes appart. \"\n        }\n      ]\n    },\n    \"frameMetricData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameMetricData\"\n        },\n        {\n          \"description\": \"Details of the metrics to request a time series of values. The metric includes the name of the frame, the aggregation type to calculate the metric value for the frame, and the thread states to use to get the count for the metric value of the frame.\"\n        }\n      ]\n    },\n    \"resolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationPeriod\"\n        },\n        {\n          \"description\": \"<p>Resolution or granularity\
  \ of the profile data used to generate the time series. This is the value used to jump through time steps in a time series. There are 3 valid values. </p> <ul> <li> <p> <code>P1D</code> \\u2014 1 day </p> </li> <li> <p> <code>PT1H</code> \\u2014 1 hour </p> </li> <li> <p> <code>PT5M</code> \\u2014 5 minutes </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The start time of the time period for the returned time series values. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \"\n        }\n      ]\n    },\n    \"unprocessedEndTimes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedEndTimeMap\"\n        },\n        {\n          \"description\": \"List of instances which remained unprocessed. This will\
  \ create a missing time step in the list of end times.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"endTime\",\n    \"endTimes\",\n    \"frameMetricData\",\n    \"resolution\",\n    \"startTime\",\n    \"unprocessedEndTimes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-batch-get-frame-metric-data-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: BatchGetFrameMetricDataResponse
---
