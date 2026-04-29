---
description: ArtifactGC describes how to delete artifacts from completed Workflows - this is embedded into the WorkflowLevelArtifactGC, and also used for individual Artifacts to override that as needed
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactGC
properties_list:
- description: PodMetadata is an optional field for specifying the Labels and Annotations that should be assigned to the Pod doing the deletion
  name: podMetadata
  type: object
- description: ServiceAccountName is an optional field for specifying the Service Account that should be assigned to the Pod doing the deletion
  name: serviceAccountName
  type: string
- description: Strategy is the strategy to use.
  name: strategy
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-gc-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifact-gc
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-artifact-gc-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-gc-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ArtifactGC\",\n  \"description\": \"ArtifactGC describes how to delete artifacts from completed Workflows - this is embedded into the WorkflowLevelArtifactGC, and also used for individual Artifacts to override that as needed\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"podMetadata\": {\n      \"description\": \"PodMetadata is an optional field for specifying the Labels and Annotations that should be assigned to the Pod doing the deletion\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Metadata\"\n    },\n    \"serviceAccountName\": {\n      \"description\": \"ServiceAccountName is an optional field for specifying the Service Account that should be assigned to\
  \ the Pod doing the deletion\",\n      \"type\": \"string\"\n    },\n    \"strategy\": {\n      \"description\": \"Strategy is the strategy to use.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-gc-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactGC
---
