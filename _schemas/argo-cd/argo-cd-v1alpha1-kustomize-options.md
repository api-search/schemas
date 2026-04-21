---
description: v1alpha1KustomizeOptions schema from Argo CD API
layout: schema
name: v1alpha1KustomizeOptions
properties_list:
- description: 'Deprecated: Use settings.Settings instead. See: settings.Settings.KustomizeVersions. If this field is set, it will be used as the Kustomize binary path. Otherwise, Versions is used.'
  name: binaryPath
  type: string
- description: ''
  name: buildOptions
  type: string
- description: Versions is a list of Kustomize versions and their corresponding binary paths and build options.
  name: versions
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-kustomize-options-schema.json
slug: argo-cd-v1alpha1-kustomize-options
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1KustomizeOptions
---
