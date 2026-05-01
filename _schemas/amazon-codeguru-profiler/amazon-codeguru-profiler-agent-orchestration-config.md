---
description: Specifies whether profiling is enabled or disabled for a profiling group. It is used by <a href="https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ConfigureAgent.html"> <code>ConfigureAgent</code> </a> to enable or disable profiling for a profiling group.
layout: schema
name: AgentOrchestrationConfig
properties_list:
- description: ''
  name: profilingEnabled
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-agent-orchestration-config-schema.json
slug: amazon-codeguru-profiler-agent-orchestration-config
source_filename: amazon-codeguru-profiler-agent-orchestration-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-agent-orchestration-config-schema.json\",\n  \"title\": \"AgentOrchestrationConfig\",\n  \"description\": \" Specifies whether profiling is enabled or disabled for a profiling group. It is used by <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ConfigureAgent.html\\\"> <code>ConfigureAgent</code> </a> to enable or disable profiling for a profiling group. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profilingEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" A <code>Boolean</code> that specifies whether the profiling agent collects profiling data or not. Set to <code>true</code> to enable profiling. \"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"profilingEnabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-agent-orchestration-config-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: AgentOrchestrationConfig
---
