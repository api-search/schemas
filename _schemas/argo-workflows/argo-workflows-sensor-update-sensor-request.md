---
description: sensor.UpdateSensorRequest schema from Argo Workflows API
layout: schema
name: sensor.UpdateSensorRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: sensor
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-sensor-update-sensor-request-schema.json
slug: argo-workflows-sensor-update-sensor-request
source_filename: argo-workflows-sensor-update-sensor-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-sensor-update-sensor-request-schema.json\",\n  \"title\": \"sensor.UpdateSensorRequest\",\n  \"description\": \"sensor.UpdateSensorRequest schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"sensor\": {\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Sensor\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-sensor-update-sensor-request-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: sensor.UpdateSensorRequest
---
