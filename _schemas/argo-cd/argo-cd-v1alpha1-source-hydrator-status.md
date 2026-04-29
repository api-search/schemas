---
description: v1alpha1SourceHydratorStatus schema from Argo CD API
layout: schema
name: v1alpha1SourceHydratorStatus
properties_list:
- description: ''
  name: currentOperation
  type: object
- description: ''
  name: lastSuccessfulOperation
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-source-hydrator-status-schema.json
slug: argo-cd-v1alpha1-source-hydrator-status
source_filename: argo-cd-v1alpha1-source-hydrator-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-source-hydrator-status-schema.json\",\n  \"title\": \"v1alpha1SourceHydratorStatus\",\n  \"description\": \"v1alpha1SourceHydratorStatus schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentOperation\": {\n      \"$ref\": \"#/definitions/v1alpha1HydrateOperation\"\n    },\n    \"lastSuccessfulOperation\": {\n      \"$ref\": \"#/definitions/v1alpha1SuccessfulHydrateOperation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-source-hydrator-status-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SourceHydratorStatus
---
