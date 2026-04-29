---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Trigger schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Trigger
properties_list:
- description: ''
  name: atLeastOnce
  type: boolean
- description: ''
  name: dlqTrigger
  type: object
- description: ''
  name: parameters
  type: array
- description: ''
  name: policy
  type: object
- description: ''
  name: rateLimit
  type: object
- description: ''
  name: retryStrategy
  type: object
- description: Template describes the trigger specification.
  name: template
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Trigger\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Trigger schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"atLeastOnce\": {\n      \"type\": \"boolean\",\n      \"title\": \"AtLeastOnce determines the trigger execution semantics.\\nDefaults to false. Trigger execution will use at-most-once semantics.\\nIf set to true, Trigger execution will switch to at-least-once semantics.\\n+kubebuilder:default=false\\n+optional\"\n    },\n    \"dlqTrigger\": {\n      \"title\": \"If the trigger fails, it will retry up to the configured number of\\nretries. If the maximum retries\
  \ are reached and the trigger is set to\\nexecute atLeastOnce, the dead letter queue (DLQ) trigger will be invoked if\\nspecified.  Invoking the dead letter queue trigger helps prevent data\\nloss.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Trigger\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"title\": \"Parameters is the list of parameters applied to the trigger template definition\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"policy\": {\n      \"title\": \"Policy to configure backoff and execution criteria for the trigger\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerPolicy\"\n    },\n    \"rateLimit\": {\n      \"title\": \"Rate limit, default unit is Second\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RateLimit\"\
  \n    },\n    \"retryStrategy\": {\n      \"title\": \"Retry strategy, defaults to no retry\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff\"\n    },\n    \"template\": {\n      \"description\": \"Template describes the trigger specification.\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerTemplate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Trigger
---
