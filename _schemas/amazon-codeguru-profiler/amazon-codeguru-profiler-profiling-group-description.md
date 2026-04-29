---
description: Contains information about a profiling group.
layout: schema
name: ProfilingGroupDescription
properties_list:
- description: ''
  name: agentOrchestrationConfig
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: computePlatform
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: profilingStatus
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-profiling-group-description-schema.json
slug: amazon-codeguru-profiler-profiling-group-description
source_filename: amazon-codeguru-profiler-profiling-group-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-profiling-group-description-schema.json\",\n  \"title\": \"ProfilingGroupDescription\",\n  \"description\": \" Contains information about a profiling group. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentOrchestrationConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentOrchestrationConfig\"\n        },\n        {\n          \"description\": \" An <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_AgentOrchestrationConfig.html\\\"> <code>AgentOrchestrationConfig</code> </a> object that indicates if the profiling group is enabled for profiled or not. \"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfilingGroupArn\"\n    \
  \    },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) identifying the profiling group resource.\"\n        }\n      ]\n    },\n    \"computePlatform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputePlatform\"\n        },\n        {\n          \"description\": \" The compute platform of the profiling group. If it is set to <code>AWSLambda</code>, then the profiled application runs on AWS Lambda. If it is set to <code>Default</code>, then the profiled application runs on a compute platform that is not AWS Lambda, such an Amazon EC2 instance, an on-premises server, or a different platform. The default is <code>Default</code>. \"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the profiling group was created. Specify using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z\
  \ represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfilingGroupName\"\n        },\n        {\n          \"description\": \"The name of the profiling group.\"\n        }\n      ]\n    },\n    \"profilingStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfilingStatus\"\n        },\n        {\n          \"description\": \" A <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ProfilingStatus.html\\\"> <code>ProfilingStatus</code> </a> object that includes information about the last time a profile agent pinged back, the last time a profile was received, and the aggregation period and start time for the most recent aggregated profile. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n         \
  \ \"description\": \" A list of the tags that belong to this profiling group. \"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time when the profiling group was last updated. Specify using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-profiling-group-description-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: ProfilingGroupDescription
---
