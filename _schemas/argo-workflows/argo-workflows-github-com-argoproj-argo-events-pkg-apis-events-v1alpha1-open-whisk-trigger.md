---
description: OpenWhiskTrigger refers to the specification of the OpenWhisk trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.OpenWhiskTrigger
properties_list:
- description: Name of the action/function.
  name: actionName
  type: string
- description: ''
  name: authToken
  type: object
- description: Host URL of the OpenWhisk.
  name: host
  type: string
- description: Namespace for the action. Defaults to "_". +optional.
  name: namespace
  type: string
- description: ''
  name: parameters
  type: array
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: ''
  name: version
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-open-whisk-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-open-whisk-trigger
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-open-whisk-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-open-whisk-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.OpenWhiskTrigger\",\n  \"description\": \"OpenWhiskTrigger refers to the specification of the OpenWhisk trigger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionName\": {\n      \"description\": \"Name of the action/function.\",\n      \"type\": \"string\"\n    },\n    \"authToken\": {\n      \"title\": \"AuthToken for authentication.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"host\": {\n      \"description\": \"Host URL of the OpenWhisk.\",\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"description\": \"Namespace for the action.\\nDefaults\
  \ to \\\"_\\\".\\n+optional.\",\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"title\": \"Parameters is the list of key-value extracted from event's payload that are applied to\\nthe trigger resource.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"payload\": {\n      \"description\": \"Payload is the list of key-value extracted from an event payload to construct the request payload.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"title\": \"Version for the API.\\nDefaults to v1.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-open-whisk-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.OpenWhiskTrigger
---
