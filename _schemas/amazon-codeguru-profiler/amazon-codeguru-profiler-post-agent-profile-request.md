---
description: The structure representing the postAgentProfileRequest.
layout: schema
name: PostAgentProfileRequest
properties_list:
- description: ''
  name: agentProfile
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-post-agent-profile-request-schema.json
slug: amazon-codeguru-profiler-post-agent-profile-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-post-agent-profile-request-schema.json\",\n  \"title\": \"PostAgentProfileRequest\",\n  \"description\": \"The structure representing the postAgentProfileRequest.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentProfile\"\n        },\n        {\n          \"description\": \" The submitted profiling data. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"agentProfile\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-post-agent-profile-request-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: PostAgentProfileRequest
---
