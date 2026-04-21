---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitArtifact schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitArtifact
properties_list:
- description: ''
  name: branch
  type: string
- description: Directory to clone the repository. We clone complete directory because GitArtifact is not limited to any specific Git service providers. Hence we don't use any specific git provider client.
  name: cloneDirectory
  type: string
- description: ''
  name: creds
  type: object
- description: ''
  name: filePath
  type: string
- description: ''
  name: insecureIgnoreHostKey
  type: boolean
- description: ''
  name: ref
  type: string
- description: ''
  name: remote
  type: object
- description: ''
  name: sshKeySecret
  type: object
- description: ''
  name: tag
  type: string
- description: ''
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-artifact-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-git-artifact
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitArtifact
---
