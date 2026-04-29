---
description: sensor.LogEntry schema from Argo Workflows API
layout: schema
name: sensor.LogEntry
properties_list:
- description: ''
  name: dependencyName
  type: string
- description: ''
  name: eventContext
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
  name: sensorName
  type: string
- description: ''
  name: time
  type: object
- description: ''
  name: triggerName
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-sensor-log-entry-schema.json
slug: argo-workflows-sensor-log-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-sensor-log-entry-schema.json\",\n  \"title\": \"sensor.LogEntry\",\n  \"description\": \"sensor.LogEntry schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dependencyName\": {\n      \"type\": \"string\",\n      \"title\": \"optional - trigger dependency name\"\n    },\n    \"eventContext\": {\n      \"type\": \"string\",\n      \"title\": \"optional - Cloud Event context\"\n    },\n    \"level\": {\n      \"type\": \"string\"\n    },\n    \"msg\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"sensorName\": {\n      \"type\": \"string\"\n    },\n    \"time\": {\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"triggerName\": {\n      \"type\": \"string\",\n\
  \      \"title\": \"optional - any trigger name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-sensor-log-entry-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: sensor.LogEntry
---
