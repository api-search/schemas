---
description: The structure representing the createProfiliingGroupRequest.
layout: schema
name: CreateProfilingGroupRequest
properties_list:
- description: ''
  name: agentOrchestrationConfig
  type: object
- description: ''
  name: computePlatform
  type: object
- description: ''
  name: profilingGroupName
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-create-profiling-group-request-schema.json
slug: amazon-codeguru-profiler-create-profiling-group-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-create-profiling-group-request-schema.json\",\n  \"title\": \"CreateProfilingGroupRequest\",\n  \"description\": \"The structure representing the createProfiliingGroupRequest.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentOrchestrationConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentOrchestrationConfig\"\n        },\n        {\n          \"description\": \" Specifies whether profiling is enabled or disabled for the created profiling group. \"\n        }\n      ]\n    },\n    \"computePlatform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputePlatform\"\n        },\n        {\n          \"description\": \" The compute platform of the profiling group. Use <code>AWSLambda</code>\
  \ if your application runs on AWS Lambda. Use <code>Default</code> if your application runs on a compute platform that is not AWS Lambda, such an Amazon EC2 instance, an on-premises server, or a different platform. If not specified, <code>Default</code> is used. \"\n        }\n      ]\n    },\n    \"profilingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfilingGroupName\"\n        },\n        {\n          \"description\": \"The name of the profiling group to create.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \" A list of tags to add to the created profiling group. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"profilingGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-create-profiling-group-request-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: CreateProfilingGroupRequest
---
