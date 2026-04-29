---
description: The part of a profile that contains a recommendation found during analysis.
layout: schema
name: Match
properties_list:
- description: ''
  name: frameAddress
  type: object
- description: ''
  name: targetFramesIndex
  type: object
- description: ''
  name: thresholdBreachValue
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-match-schema.json
slug: amazon-codeguru-profiler-match
source_filename: amazon-codeguru-profiler-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-match-schema.json\",\n  \"title\": \"Match\",\n  \"description\": \"The part of a profile that contains a recommendation found during analysis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"frameAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The location in the profiling graph that contains a recommendation found during analysis.\"\n        }\n      ]\n    },\n    \"targetFramesIndex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The target frame that triggered a match.\"\n        }\n      ]\n    },\n    \"thresholdBreachValue\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The value in the profile data that exceeded the recommendation threshold.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-match-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: Match
---
