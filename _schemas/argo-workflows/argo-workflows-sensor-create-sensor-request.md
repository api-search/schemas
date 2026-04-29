---
description: sensor.CreateSensorRequest schema from Argo Workflows API
layout: schema
name: sensor.CreateSensorRequest
properties_list:
- description: ''
  name: createOptions
  type: object
- description: ''
  name: namespace
  type: string
- description: ''
  name: sensor
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-sensor-create-sensor-request-schema.json
slug: argo-workflows-sensor-create-sensor-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-sensor-create-sensor-request-schema.json\",\n  \"title\": \"sensor.CreateSensorRequest\",\n  \"description\": \"sensor.CreateSensorRequest schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createOptions\": {\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.CreateOptions\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"sensor\": {\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Sensor\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-sensor-create-sensor-request-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: sensor.CreateSensorRequest
---
