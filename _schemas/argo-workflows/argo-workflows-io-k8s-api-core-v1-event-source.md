---
description: EventSource contains information for an event.
layout: schema
name: io.k8s.api.core.v1.EventSource
properties_list:
- description: Component from which the event is generated.
  name: component
  type: string
- description: Node name on which the event is generated.
  name: host
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-event-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-event-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-event-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.EventSource\",\n  \"description\": \"EventSource contains information for an event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"component\": {\n      \"description\": \"Component from which the event is generated.\",\n      \"type\": \"string\"\n    },\n    \"host\": {\n      \"description\": \"Node name on which the event is generated.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.EventSource
---
