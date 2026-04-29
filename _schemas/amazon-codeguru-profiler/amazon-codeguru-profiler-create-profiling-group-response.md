---
description: The structure representing the createProfilingGroupResponse.
layout: schema
name: CreateProfilingGroupResponse
properties_list:
- description: ''
  name: profilingGroup
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-create-profiling-group-response-schema.json
slug: amazon-codeguru-profiler-create-profiling-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-create-profiling-group-response-schema.json\",\n  \"title\": \"CreateProfilingGroupResponse\",\n  \"description\": \"The structure representing the createProfilingGroupResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profilingGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfilingGroupDescription\"\n        },\n        {\n          \"description\": \" The returned <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ProfilingGroupDescription.html\\\"> <code>ProfilingGroupDescription</code> </a> object that contains information about the created profiling group. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"profilingGroup\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-create-profiling-group-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: CreateProfilingGroupResponse
---
