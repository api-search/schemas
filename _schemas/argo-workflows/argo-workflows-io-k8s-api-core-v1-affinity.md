---
description: Affinity is a group of affinity scheduling rules.
layout: schema
name: io.k8s.api.core.v1.Affinity
properties_list:
- description: Describes node affinity scheduling rules for the pod.
  name: nodeAffinity
  type: object
- description: Describes pod affinity scheduling rules (e.g. co-locate this pod in the same node, zone, etc. as some other pod(s)).
  name: podAffinity
  type: object
- description: Describes pod anti-affinity scheduling rules (e.g. avoid putting this pod in the same node, zone, etc. as some other pod(s)).
  name: podAntiAffinity
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-affinity-schema.json
slug: argo-workflows-io-k8s-api-core-v1-affinity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-affinity-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.Affinity\",\n  \"description\": \"Affinity is a group of affinity scheduling rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nodeAffinity\": {\n      \"description\": \"Describes node affinity scheduling rules for the pod.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.NodeAffinity\"\n    },\n    \"podAffinity\": {\n      \"description\": \"Describes pod affinity scheduling rules (e.g. co-locate this pod in the same node, zone, etc. as some other pod(s)).\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PodAffinity\"\n    },\n    \"podAntiAffinity\": {\n      \"description\": \"Describes pod anti-affinity scheduling rules (e.g. avoid putting this pod in the same node, zone, etc. as some\
  \ other pod(s)).\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PodAntiAffinity\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-affinity-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.Affinity
---
