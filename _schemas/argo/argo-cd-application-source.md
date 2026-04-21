---
description: Git or Helm chart source for the application manifests.
layout: schema
name: ApplicationSource
properties_list:
- description: URL of the Git repository or Helm chart repository.
  name: repoURL
  type: string
- description: Path within the repository where manifests are located. Used for Git repositories.
  name: path
  type: string
- description: Git branch, tag, or commit SHA to deploy. Defaults to HEAD.
  name: targetRevision
  type: string
- description: Helm chart name. Used when repoURL points to a Helm registry.
  name: chart
  type: string
- description: Helm-specific source configuration.
  name: helm
  type: object
- description: Kustomize-specific source configuration.
  name: kustomize
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-application-source-schema.json
slug: argo-cd-application-source
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ApplicationSource
---
