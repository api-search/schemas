---
description: The structure representing the updateProfilingGroupResponse.
layout: schema
name: UpdateProfilingGroupResponse
properties_list:
- description: ''
  name: profilingGroup
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-update-profiling-group-response-schema.json
slug: amazon-codeguru-profiler-update-profiling-group-response
source_filename: amazon-codeguru-profiler-update-profiling-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-update-profiling-group-response-schema.json\",\n  \"title\": \"UpdateProfilingGroupResponse\",\n  \"description\": \"The structure representing the updateProfilingGroupResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profilingGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfilingGroupDescription\"\n        },\n        {\n          \"description\": \" A <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ProfilingGroupDescription.html\\\"> <code>ProfilingGroupDescription</code> </a> that contains information about the returned updated profiling group. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"profilingGroup\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-update-profiling-group-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: UpdateProfilingGroupResponse
---
