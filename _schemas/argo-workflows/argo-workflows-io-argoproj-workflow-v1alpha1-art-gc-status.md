---
description: ArtGCStatus maintains state related to ArtifactGC
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtGCStatus
properties_list:
- description: if this is true, we already checked to see if we need to do it and we don't
  name: notSpecified
  type: boolean
- description: have completed Pods been processed? (mapped by Pod name) used to prevent re-processing the Status of a Pod more than once
  name: podsRecouped
  type: object
- description: have Pods been started to perform this strategy? (enables us not to re-process what we've already done)
  name: strategiesProcessed
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-art-gc-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-art-gc-status
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-art-gc-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-art-gc-status-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ArtGCStatus\",\n  \"description\": \"ArtGCStatus maintains state related to ArtifactGC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notSpecified\": {\n      \"description\": \"if this is true, we already checked to see if we need to do it and we don't\",\n      \"type\": \"boolean\"\n    },\n    \"podsRecouped\": {\n      \"description\": \"have completed Pods been processed? (mapped by Pod name) used to prevent re-processing the Status of a Pod more than once\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\n      }\n    },\n    \"strategiesProcessed\": {\n      \"description\": \"have Pods been started to perform this strategy?\
  \ (enables us not to re-process what we've already done)\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-art-gc-status-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtGCStatus
---
