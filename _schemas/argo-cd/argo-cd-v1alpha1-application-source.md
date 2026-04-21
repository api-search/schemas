---
description: v1alpha1ApplicationSource schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSource
properties_list:
- description: Chart is a Helm chart name, and must be specified for applications sourced from a Helm repo.
  name: chart
  type: string
- description: ''
  name: directory
  type: object
- description: ''
  name: helm
  type: object
- description: ''
  name: kustomize
  type: object
- description: Name is used to refer to a source and is displayed in the UI. It is used in multi-source Applications.
  name: name
  type: string
- description: Path is a directory path within the Git repository, and is only valid for applications sourced from Git.
  name: path
  type: string
- description: ''
  name: plugin
  type: object
- description: Ref is reference to another source within sources field. This field will not be used if used with a `source` tag.
  name: ref
  type: string
- description: ''
  name: repoURL
  type: string
- description: 'TargetRevision defines the revision of the source to sync the application to. In case of Git, this can be commit, tag, or branch. If omitted, will equal to HEAD. In case of Helm, this is a semver tag '
  name: targetRevision
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-source-schema.json
slug: argo-cd-v1alpha1-application-source
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSource
---
