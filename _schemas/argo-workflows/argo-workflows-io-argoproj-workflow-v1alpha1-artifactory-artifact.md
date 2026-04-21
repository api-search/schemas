---
description: ArtifactoryArtifact is the location of an artifactory artifact
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactoryArtifact
properties_list:
- description: PasswordSecret is the secret selector to the repository password
  name: passwordSecret
  type: object
- description: URL of the artifact
  name: url
  type: string
- description: UsernameSecret is the secret selector to the repository username
  name: usernameSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactoryArtifact
---
