---
description: Information about potential recommendations that might be created from the analysis of profiling data.
layout: schema
name: FindingsReportSummary
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: profileEndTime
  type: object
- description: ''
  name: profileStartTime
  type: object
- description: ''
  name: profilingGroupName
  type: object
- description: ''
  name: totalNumberOfFindings
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-findings-report-summary-schema.json
slug: amazon-codeguru-profiler-findings-report-summary
source_filename: amazon-codeguru-profiler-findings-report-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-findings-report-summary-schema.json\",\n  \"title\": \"FindingsReportSummary\",\n  \"description\": \" Information about potential recommendations that might be created from the analysis of profiling data. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingsReportId\"\n        },\n        {\n          \"description\": \"The universally unique identifier (UUID) of the recommendation report.\"\n        }\n      ]\n    },\n    \"profileEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The end time of the period during which the metric is flagged as anomalous. This is specified\
  \ using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \"\n        }\n      ]\n    },\n    \"profileStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start time of the profile the analysis data is about. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC.\"\n        }\n      ]\n    },\n    \"profilingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the profiling group that is associated with the analysis data.\"\n        }\n      ]\n    },\n    \"totalNumberOfFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"\
  The total number of different recommendations that were found by the analysis.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-findings-report-summary-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: FindingsReportSummary
---
