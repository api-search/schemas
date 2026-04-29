---
description: VolumeClaimGC describes how to delete volumes from completed Workflows
layout: schema
name: io.argoproj.workflow.v1alpha1.VolumeClaimGC
properties_list:
- description: Strategy is the strategy to use. One of "OnWorkflowCompletion", "OnWorkflowSuccess". Defaults to "OnWorkflowSuccess"
  name: strategy
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-volume-claim-gc-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-volume-claim-gc
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-volume-claim-gc-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-volume-claim-gc-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.VolumeClaimGC\",\n  \"description\": \"VolumeClaimGC describes how to delete volumes from completed Workflows\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"strategy\": {\n      \"description\": \"Strategy is the strategy to use. One of \\\"OnWorkflowCompletion\\\", \\\"OnWorkflowSuccess\\\". Defaults to \\\"OnWorkflowSuccess\\\"\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-volume-claim-gc-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.VolumeClaimGC
---
