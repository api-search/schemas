---
description: sensor.SensorWatchEvent schema from Argo Workflows API
layout: schema
name: sensor.SensorWatchEvent
properties_list:
- description: ''
  name: object
  type: object
- description: ''
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-sensor-sensor-watch-event-schema.json
slug: argo-workflows-sensor-sensor-watch-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-sensor-sensor-watch-event-schema.json\",\n  \"title\": \"sensor.SensorWatchEvent\",\n  \"description\": \"sensor.SensorWatchEvent schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Sensor\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-sensor-sensor-watch-event-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: sensor.SensorWatchEvent
---
