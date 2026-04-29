---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.MNSEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.MNSEventSource
properties_list:
- description: ''
  name: accessKey
  type: object
- description: ''
  name: endpoint
  type: string
- description: ''
  name: filter
  type: object
- description: ''
  name: jsonBody
  type: boolean
- description: ''
  name: queue
  type: string
- description: ''
  name: secretKey
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-mns-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-mns-event-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-mns-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.MNSEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.MNSEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessKey\": {\n      \"title\": \"AccessKey refers K8s secret containing AlibabaCloud access key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"title\": \"Endpoint configures connection to a specific AlibabaCloud MNS endpoint\\n+optional\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\
  \n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"+optional\"\n    },\n    \"queue\": {\n      \"type\": \"string\",\n      \"title\": \"Queue is AlibabaCloud MNS queue to listen to for messages\"\n    },\n    \"secretKey\": {\n      \"title\": \"SecretKey refers K8s secret containing AlibabaCloud secret key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-mns-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.MNSEventSource
---
