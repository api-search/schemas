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
