---
description: v1alpha1KustomizeReplica schema from Argo CD API
layout: schema
name: v1alpha1KustomizeReplica
properties_list:
- description: ''
  name: count
  type: object
- description: ''
  name: name
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-kustomize-replica-schema.json
slug: argo-cd-v1alpha1-kustomize-replica
source_filename: argo-cd-v1alpha1-kustomize-replica-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-replica-schema.json\",\n  \"title\": \"v1alpha1KustomizeReplica\",\n  \"description\": \"v1alpha1KustomizeReplica schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"$ref\": \"#/definitions/intstrIntOrString\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name of Deployment or StatefulSet\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-kustomize-replica-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1KustomizeReplica
---
