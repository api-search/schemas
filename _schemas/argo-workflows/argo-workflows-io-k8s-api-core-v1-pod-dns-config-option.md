---
description: PodDNSConfigOption defines DNS resolver options of a pod.
layout: schema
name: io.k8s.api.core.v1.PodDNSConfigOption
properties_list:
- description: Name is this DNS resolver option's name. Required.
  name: name
  type: string
- description: Value is this DNS resolver option's value.
  name: value
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-pod-dns-config-option-schema.json
slug: argo-workflows-io-k8s-api-core-v1-pod-dns-config-option
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-pod-dns-config-option-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PodDNSConfigOption\",\n  \"description\": \"PodDNSConfigOption defines DNS resolver options of a pod.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name is this DNS resolver option's name. Required.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Value is this DNS resolver option's value.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-pod-dns-config-option-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PodDNSConfigOption
---
