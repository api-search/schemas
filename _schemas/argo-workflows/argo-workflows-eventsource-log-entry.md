---
description: eventsource.LogEntry schema from Argo Workflows API
layout: schema
name: eventsource.LogEntry
properties_list:
- description: ''
  name: eventName
  type: string
- description: ''
  name: eventSourceName
  type: string
- description: ''
  name: eventSourceType
  type: string
- description: ''
  name: level
  type: string
- description: ''
  name: msg
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: time
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-eventsource-log-entry-schema.json
slug: argo-workflows-eventsource-log-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-eventsource-log-entry-schema.json\",\n  \"title\": \"eventsource.LogEntry\",\n  \"description\": \"eventsource.LogEntry schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventName\": {\n      \"type\": \"string\",\n      \"title\": \"optional - the event name (e.g. `example`)\"\n    },\n    \"eventSourceName\": {\n      \"type\": \"string\"\n    },\n    \"eventSourceType\": {\n      \"type\": \"string\",\n      \"title\": \"optional - the event source type (e.g. `webhook`)\"\n    },\n    \"level\": {\n      \"type\": \"string\"\n    },\n    \"msg\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"time\": {\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-eventsource-log-entry-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: eventsource.LogEntry
---
