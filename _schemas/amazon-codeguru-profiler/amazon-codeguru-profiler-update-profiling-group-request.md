---
description: The structure representing the updateProfilingGroupRequest.
layout: schema
name: UpdateProfilingGroupRequest
properties_list:
- description: ''
  name: agentOrchestrationConfig
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-update-profiling-group-request-schema.json
slug: amazon-codeguru-profiler-update-profiling-group-request
source_filename: amazon-codeguru-profiler-update-profiling-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-update-profiling-group-request-schema.json\",\n  \"title\": \"UpdateProfilingGroupRequest\",\n  \"description\": \"The structure representing the updateProfilingGroupRequest.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentOrchestrationConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentOrchestrationConfig\"\n        },\n        {\n          \"description\": \" Specifies whether profiling is enabled or disabled for a profiling group. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"agentOrchestrationConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-update-profiling-group-request-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: UpdateProfilingGroupRequest
---
