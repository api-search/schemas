---
description: SleepAction describes a "sleep" action.
layout: schema
name: io.k8s.api.core.v1.SleepAction
properties_list:
- description: Seconds is the number of seconds to sleep.
  name: seconds
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-sleep-action-schema.json
slug: argo-workflows-io-k8s-api-core-v1-sleep-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-sleep-action-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.SleepAction\",\n  \"description\": \"SleepAction describes a \\\"sleep\\\" action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"seconds\": {\n      \"description\": \"Seconds is the number of seconds to sleep.\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"seconds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-sleep-action-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.SleepAction
---
