---
description: The structure representing the GetRecommendationsResponse.
layout: schema
name: GetRecommendationsResponse
properties_list:
- description: ''
  name: anomalies
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
  name: recommendations
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-get-recommendations-response-schema.json
slug: amazon-codeguru-profiler-get-recommendations-response
source_filename: amazon-codeguru-profiler-get-recommendations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-get-recommendations-response-schema.json\",\n  \"title\": \"GetRecommendationsResponse\",\n  \"description\": \"The structure representing the GetRecommendationsResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"anomalies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Anomalies\"\n        },\n        {\n          \"description\": \" The list of anomalies that the analysis has found for this profile. \"\n        }\n      ]\n    },\n    \"profileEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The end time of the profile the analysis data is about. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z\
  \ represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \"\n        }\n      ]\n    },\n    \"profileStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The start time of the profile the analysis data is about. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \"\n        }\n      ]\n    },\n    \"profilingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfilingGroupName\"\n        },\n        {\n          \"description\": \"The name of the profiling group the analysis data is about.\"\n        }\n      ]\n    },\n    \"recommendations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Recommendations\"\n        },\n        {\n          \"description\": \"The list of recommendations that the analysis found for this profile.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"anomalies\",\n    \"profileEndTime\",\n    \"profileStartTime\",\n    \"profilingGroupName\",\n    \"recommendations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-get-recommendations-response-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: GetRecommendationsResponse
---
