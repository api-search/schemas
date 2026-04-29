---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SensorSpec schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SensorSpec
properties_list:
- description: Dependencies is a list of the events that this sensor is dependent on.
  name: dependencies
  type: array
- description: ErrorOnFailedRound if set to true, marks sensor state as `error` if the previous trigger round fails. Once sensor state is set to `error`, no further triggers will be processed.
  name: errorOnFailedRound
  type: boolean
- description: ''
  name: eventBusName
  type: string
- description: ''
  name: loggingFields
  type: object
- description: ''
  name: replicas
  type: integer
- description: ''
  name: revisionHistoryLimit
  type: integer
- description: ''
  name: template
  type: object
- description: Triggers is a list of the things that this sensor evokes. These are the outputs from this sensor.
  name: triggers
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sensor-spec-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sensor-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sensor-spec-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SensorSpec\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SensorSpec schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dependencies\": {\n      \"description\": \"Dependencies is a list of the events that this sensor is dependent on.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventDependency\"\n      }\n    },\n    \"errorOnFailedRound\": {\n      \"description\": \"ErrorOnFailedRound if set to true, marks sensor state as `error` if the previous trigger round fails.\\\
  nOnce sensor state is set to `error`, no further triggers will be processed.\",\n      \"type\": \"boolean\"\n    },\n    \"eventBusName\": {\n      \"type\": \"string\",\n      \"title\": \"EventBusName references to a EventBus name. By default the value is \\\"default\\\"\"\n    },\n    \"loggingFields\": {\n      \"type\": \"object\",\n      \"title\": \"LoggingFields add additional key-value pairs when logging happens\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"replicas\": {\n      \"type\": \"integer\",\n      \"title\": \"Replicas is the sensor deployment replicas\"\n    },\n    \"revisionHistoryLimit\": {\n      \"type\": \"integer\",\n      \"title\": \"RevisionHistoryLimit specifies how many old deployment revisions to retain\\n+optional\"\n    },\n    \"template\": {\n      \"title\": \"Template is the pod specification for the sensor\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Template\"\
  \n    },\n    \"triggers\": {\n      \"description\": \"Triggers is a list of the things that this sensor evokes. These are the outputs from this sensor.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Trigger\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sensor-spec-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SensorSpec
---
