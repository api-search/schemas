---
description: ArtifactRepositoryRefStatus is the resolved artifact repository reference with namespace io.argoproj.workflow.v1alpha1.
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactRepositoryRefStatus
properties_list:
- description: The repository the workflow will use. This maybe empty before v3.1.
  name: artifactRepository
  type: object
- description: The name of the config map. Defaults to "artifact-repositories".
  name: configMap
  type: string
- description: If this ref represents the default artifact repository, rather than a config map.
  name: default
  type: boolean
- description: The config map key. Defaults to the value of the "workflows.argoproj.io/default-artifact-repository" annotation.
  name: key
  type: string
- description: The namespace of the config map. Defaults to the workflow's namespace, or the controller's namespace (if found).
  name: namespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-repository-ref-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifact-repository-ref-status
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactRepositoryRefStatus
---
