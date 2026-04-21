---
description: ArtifactoryArtifactRepository defines the controller configuration for an artifactory artifact repository
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactoryArtifactRepository
properties_list:
- description: KeyFormat defines the format of how to store keys and can reference workflow variables.
  name: keyFormat
  type: string
- description: PasswordSecret is the secret selector to the repository password
  name: passwordSecret
  type: object
- description: RepoURL is the url for artifactory repo.
  name: repoURL
  type: string
- description: UsernameSecret is the secret selector to the repository username
  name: usernameSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-repository-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-repository
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactoryArtifactRepository
---
