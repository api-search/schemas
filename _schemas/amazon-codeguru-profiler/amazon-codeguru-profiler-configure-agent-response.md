---
description: The structure representing the configureAgentResponse.
layout: schema
name: ConfigureAgentResponse
properties_list:
- description: ''
  name: configuration
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-configure-agent-response-schema.json
slug: amazon-codeguru-profiler-configure-agent-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-configure-agent-response-schema.json\",\n  \"title\": \"ConfigureAgentResponse\",\n  \"description\": \"The structure representing the configureAgentResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentConfiguration\"\n        },\n        {\n          \"description\": \" An <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_AgentConfiguration.html\\\"> <code>AgentConfiguration</code> </a> object that specifies if an agent profiles or not and for how long to return profiling data. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"configuration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-configure-agent-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: ConfigureAgentResponse
---
