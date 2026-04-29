---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerPolicy schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerPolicy
properties_list:
- description: ''
  name: k8s
  type: object
- description: ''
  name: status
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-policy-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-policy
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-policy-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerPolicy\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerPolicy schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"k8s\": {\n      \"title\": \"K8SResourcePolicy refers to the policy used to check the state of K8s based triggers using using labels\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.K8SResourcePolicy\"\n    },\n    \"status\": {\n      \"title\": \"Status refers to the policy used to check the state of the trigger using response status\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StatusPolicy\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-policy-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerPolicy
---
