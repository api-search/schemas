---
description: Specifies the aggregation period and aggregation start time for an aggregated profile. An aggregated profile is used to collect posted agent profiles during an aggregation period. There are three possible aggregation periods (1 day, 1 hour, or 5 minutes).
layout: schema
name: AggregatedProfileTime
properties_list:
- description: ''
  name: period
  type: object
- description: ''
  name: start
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-aggregated-profile-time-schema.json
slug: amazon-codeguru-profiler-aggregated-profile-time
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-aggregated-profile-time-schema.json\",\n  \"title\": \"AggregatedProfileTime\",\n  \"description\": \" Specifies the aggregation period and aggregation start time for an aggregated profile. An aggregated profile is used to collect posted agent profiles during an aggregation period. There are three possible aggregation periods (1 day, 1 hour, or 5 minutes). \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"period\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationPeriod\"\n        },\n        {\n          \"description\": \"<p> The aggregation period. This indicates the period during which an aggregation profile collects posted agent profiles for a profiling group. Use one of three valid durations that are specified using the\
  \ ISO 8601 format. </p> <ul> <li> <p> <code>P1D</code> \\u2014 1 day </p> </li> <li> <p> <code>PT1H</code> \\u2014 1 hour </p> </li> <li> <p> <code>PT5M</code> \\u2014 5 minutes </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"start\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p> The time that aggregation of posted agent profiles for a profiling group starts. The aggregation profile contains profiles posted by the agent starting at this time for an aggregation period specified by the <code>period</code> property of the <code>AggregatedProfileTime</code> object. </p> <p> Specify <code>start</code> using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-aggregated-profile-time-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: AggregatedProfileTime
---
