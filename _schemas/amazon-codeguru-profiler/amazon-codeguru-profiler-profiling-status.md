---
description: Profiling status includes information about the last time a profile agent pinged back, the last time a profile was received, and the aggregation period and start time for the most recent aggregated profile.
layout: schema
name: ProfilingStatus
properties_list:
- description: ''
  name: latestAgentOrchestratedAt
  type: object
- description: ''
  name: latestAgentProfileReportedAt
  type: object
- description: ''
  name: latestAggregatedProfile
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-profiling-status-schema.json
slug: amazon-codeguru-profiler-profiling-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-profiling-status-schema.json\",\n  \"title\": \"ProfilingStatus\",\n  \"description\": \" Profiling status includes information about the last time a profile agent pinged back, the last time a profile was received, and the aggregation period and start time for the most recent aggregated profile. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latestAgentOrchestratedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the profiling agent most recently pinged back. Specify using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC.\"\n        }\n      ]\n    },\n    \"latestAgentProfileReportedAt\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the most recent profile was received. Specify using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC.\"\n        }\n      ]\n    },\n    \"latestAggregatedProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedProfileTime\"\n        },\n        {\n          \"description\": \" An <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_AggregatedProfileTime.html\\\"> <code>AggregatedProfileTime</code> </a> object that contains the aggregation period and start time for an aggregated profile. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-profiling-status-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: ProfilingStatus
---
