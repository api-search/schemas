---
description: Information about the integration of DevOps Guru as consumer with another AWS service, such as AWS CodeGuru Profiler via EventBridge.
layout: schema
name: EventSourcesConfig
properties_list:
- description: ''
  name: AmazonCodeGuruProfiler
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-event-sources-config-schema.json
slug: amazon-devops-guru-event-sources-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-event-sources-config-schema.json\",\n  \"title\": \"EventSourcesConfig\",\n  \"description\": \"Information about the integration of DevOps Guru as consumer with another AWS service, such as AWS CodeGuru Profiler via EventBridge.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AmazonCodeGuruProfiler\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonCodeGuruProfilerIntegration\"\n        },\n        {\n          \"description\": \"Information about whether DevOps Guru is configured to consume recommendations which are generated from AWS CodeGuru Profiler.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-event-sources-config-schema.json
tags:
- Anomaly Detection
- AWS
- DevOps
- Machine Learning
- Operational Intelligence
title: EventSourcesConfig
---
