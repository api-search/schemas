---
description: SourceHydrator specifies a dry "don't repeat yourself" source for manifests, a sync source from which to sync hydrated manifests, and an optional hydrateTo location to act as a "staging" aread for hydrated manifests.
layout: schema
name: v1alpha1SourceHydrator
properties_list:
- description: ''
  name: drySource
  type: object
- description: ''
  name: hydrateTo
  type: object
- description: ''
  name: syncSource
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-source-hydrator-schema.json
slug: argo-cd-v1alpha1-source-hydrator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-source-hydrator-schema.json\",\n  \"title\": \"v1alpha1SourceHydrator\",\n  \"description\": \"SourceHydrator specifies a dry \\\"don't repeat yourself\\\" source for manifests, a sync source from which to sync\\nhydrated manifests, and an optional hydrateTo location to act as a \\\"staging\\\" aread for hydrated manifests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"drySource\": {\n      \"$ref\": \"#/definitions/v1alpha1DrySource\"\n    },\n    \"hydrateTo\": {\n      \"$ref\": \"#/definitions/v1alpha1HydrateTo\"\n    },\n    \"syncSource\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncSource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-source-hydrator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SourceHydrator
---
