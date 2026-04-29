---
description: v1alpha1ApplicationSetRolloutStep schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSetRolloutStep
properties_list:
- description: ''
  name: matchExpressions
  type: array
- description: ''
  name: maxUpdate
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-rollout-step-schema.json
slug: argo-cd-v1alpha1-application-set-rollout-step
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-rollout-step-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetRolloutStep\",\n  \"description\": \"v1alpha1ApplicationSetRolloutStep schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchExpressions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationMatchExpression\"\n      }\n    },\n    \"maxUpdate\": {\n      \"$ref\": \"#/definitions/intstrIntOrString\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-rollout-step-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetRolloutStep
---
