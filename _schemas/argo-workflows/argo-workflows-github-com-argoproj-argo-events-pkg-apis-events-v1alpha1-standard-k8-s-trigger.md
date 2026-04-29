---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StandardK8STrigger schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StandardK8STrigger
properties_list:
- description: ''
  name: liveObject
  type: boolean
- description: ''
  name: operation
  type: string
- description: Parameters is the list of parameters that is applied to resolved K8s trigger object.
  name: parameters
  type: array
- description: ''
  name: patchStrategy
  type: string
- description: ''
  name: source
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-standard-k8-s-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-standard-k8-s-trigger
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-standard-k8-s-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-standard-k8-s-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StandardK8STrigger\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StandardK8STrigger schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"liveObject\": {\n      \"type\": \"boolean\",\n      \"title\": \"LiveObject specifies whether the resource should be directly fetched from K8s instead\\nof being marshaled from the resource artifact. If set to true, the resource artifact\\nmust contain the information required to uniquely identify the resource in the cluster,\\nthat is, you must specify \\\"apiVersion\\\", \\\"kind\\\" as well as \\\"name\\\" and \\\"namespace\\\
  \" meta\\ndata.\\nOnly valid for operation type `update`\\n+optional\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"title\": \"Operation refers to the type of operation performed on the k8s resource.\\nDefault value is Create.\\n+optional\"\n    },\n    \"parameters\": {\n      \"description\": \"Parameters is the list of parameters that is applied to resolved K8s trigger object.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"patchStrategy\": {\n      \"type\": \"string\",\n      \"title\": \"PatchStrategy controls the K8s object patching strategy when the trigger operation is specified as patch.\\npossible values:\\n\\\"application/json-patch+json\\\"\\n\\\"application/merge-patch+json\\\"\\n\\\"application/strategic-merge-patch+json\\\"\\n\\\"application/apply-patch+yaml\\\".\\nDefaults to \\\"application/merge-patch+json\\\"\
  \\n+optional\"\n    },\n    \"source\": {\n      \"title\": \"Source of the K8s resource file(s)\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArtifactLocation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-standard-k8-s-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StandardK8STrigger
---
