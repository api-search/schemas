---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.K8SResourcePolicy schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.K8SResourcePolicy
properties_list:
- description: ''
  name: backoff
  type: object
- description: ''
  name: errorOnBackoffTimeout
  type: boolean
- description: ''
  name: labels
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-k8-s-resource-policy-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-k8-s-resource-policy
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-k8-s-resource-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-k8-s-resource-policy-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.K8SResourcePolicy\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.K8SResourcePolicy schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"backoff\": {\n      \"title\": \"Backoff before checking resource state\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff\"\n    },\n    \"errorOnBackoffTimeout\": {\n      \"type\": \"boolean\",\n      \"title\": \"ErrorOnBackoffTimeout determines whether sensor should transition to error state if the trigger policy is unable to determine\\nthe state of the resource\"\n   \
  \ },\n    \"labels\": {\n      \"type\": \"object\",\n      \"title\": \"Labels required to identify whether a resource is in success state\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-k8-s-resource-policy-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.K8SResourcePolicy
---
