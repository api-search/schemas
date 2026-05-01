---
description: Contains the start time of a profile.
layout: schema
name: ProfileTime
properties_list:
- description: ''
  name: start
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-profile-time-schema.json
slug: amazon-codeguru-profiler-profile-time
source_filename: amazon-codeguru-profiler-profile-time-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-profile-time-schema.json\",\n  \"title\": \"ProfileTime\",\n  \"description\": \" Contains the start time of a profile. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start time of a profile. It is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-profile-time-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: ProfileTime
---
