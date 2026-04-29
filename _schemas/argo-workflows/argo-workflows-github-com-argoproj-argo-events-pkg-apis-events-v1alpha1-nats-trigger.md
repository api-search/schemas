---
description: NATSTrigger refers to the specification of the NATS trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSTrigger
properties_list:
- description: ''
  name: auth
  type: object
- description: ''
  name: parameters
  type: array
- description: ''
  name: payload
  type: array
- description: Name of the subject to put message on.
  name: subject
  type: string
- description: ''
  name: tls
  type: object
- description: URL of the NATS cluster.
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-trigger
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSTrigger\",\n  \"description\": \"NATSTrigger refers to the specification of the NATS trigger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"auth\": {\n      \"title\": \"AuthInformation\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSAuth\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"payload\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\
  \n      }\n    },\n    \"subject\": {\n      \"description\": \"Name of the subject to put message on.\",\n      \"type\": \"string\"\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the NATS producer.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"url\": {\n      \"description\": \"URL of the NATS cluster.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSTrigger
---
