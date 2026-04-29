---
description: PluginArtifactRepository defines the controller configuration for a plugin artifact repository
layout: schema
name: io.argoproj.workflow.v1alpha1.PluginArtifactRepository
properties_list:
- description: ''
  name: configuration
  type: string
- description: ''
  name: keyFormat
  type: string
- description: ''
  name: name
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-plugin-artifact-repository-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-plugin-artifact-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-plugin-artifact-repository-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.PluginArtifactRepository\",\n  \"description\": \"PluginArtifactRepository defines the controller configuration for a plugin artifact repository\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"type\": \"string\"\n    },\n    \"keyFormat\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"configuration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-plugin-artifact-repository-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.PluginArtifactRepository
---
