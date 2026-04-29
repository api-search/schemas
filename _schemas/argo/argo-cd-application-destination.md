---
description: Target Kubernetes cluster and namespace for application deployment.
layout: schema
name: ApplicationDestination
properties_list:
- description: Kubernetes API server URL of the target cluster. Use https://kubernetes.default.svc for the in-cluster target.
  name: server
  type: string
- description: Name of the registered cluster. Mutually exclusive with server.
  name: name
  type: string
- description: Target namespace in the destination cluster.
  name: namespace
  type: string
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-application-destination-schema.json
slug: argo-cd-application-destination
source_filename: argo-cd-application-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-destination-schema.json\",\n  \"title\": \"ApplicationDestination\",\n  \"description\": \"Target Kubernetes cluster and namespace for application deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"server\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes API server URL of the target cluster. Use https://kubernetes.default.svc for the in-cluster target.\",\n      \"format\": \"uri\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the registered cluster. Mutually exclusive with server.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Target namespace in the destination cluster.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-destination-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ApplicationDestination
---
