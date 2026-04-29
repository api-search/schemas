---
description: The structure representing the getProfileResponse.
layout: schema
name: GetProfileResponse
properties_list:
- description: ''
  name: profile
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-get-profile-response-schema.json
slug: amazon-codeguru-profiler-get-profile-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-get-profile-response-schema.json\",\n  \"title\": \"GetProfileResponse\",\n  \"description\": \"The structure representing the getProfileResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedProfile\"\n        },\n        {\n          \"description\": \"Information about the profile.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"profile\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-get-profile-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: GetProfileResponse
---
