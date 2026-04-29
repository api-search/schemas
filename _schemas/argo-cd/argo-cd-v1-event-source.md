---
description: EventSource contains information for an event.
layout: schema
name: v1EventSource
properties_list:
- description: ''
  name: component
  type: string
- description: ''
  name: host
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-event-source-schema.json
slug: argo-cd-v1-event-source
source_filename: argo-cd-v1-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-event-source-schema.json\",\n  \"title\": \"v1EventSource\",\n  \"description\": \"EventSource contains information for an event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"component\": {\n      \"type\": \"string\",\n      \"title\": \"Component from which the event is generated.\\n+optional\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"title\": \"Node name on which the event is generated.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-event-source-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1EventSource
---
