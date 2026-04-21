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
