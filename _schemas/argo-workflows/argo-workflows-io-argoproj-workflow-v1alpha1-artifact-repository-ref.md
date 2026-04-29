---
description: ArtifactRepositoryRef is a reference to an artifact repository config map.
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactRepositoryRef
properties_list:
- description: The name of the config map. Defaults to "artifact-repositories".
  name: configMap
  type: string
- description: The config map key. Defaults to the value of the "workflows.argoproj.io/default-artifact-repository" annotation.
  name: key
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-repository-ref-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifact-repository-ref
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-repository-ref-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ArtifactRepositoryRef\",\n  \"description\": \"ArtifactRepositoryRef is a reference to an artifact repository config map.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configMap\": {\n      \"description\": \"The name of the config map. Defaults to \\\"artifact-repositories\\\".\",\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"description\": \"The config map key. Defaults to the value of the \\\"workflows.argoproj.io/default-artifact-repository\\\" annotation.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-repository-ref-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactRepositoryRef
---
