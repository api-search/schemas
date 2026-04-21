---
description: v1alpha1ApplicationSourceKustomize schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSourceKustomize
properties_list:
- description: APIVersions specifies the Kubernetes resource API versions to pass to Helm when templating manifests. By default, Argo CD uses the API versions of the target cluster. The format is [group/]version/kin
  name: apiVersions
  type: array
- description: ''
  name: commonAnnotations
  type: object
- description: ''
  name: commonAnnotationsEnvsubst
  type: boolean
- description: ''
  name: commonLabels
  type: object
- description: ''
  name: components
  type: array
- description: ''
  name: forceCommonAnnotations
  type: boolean
- description: ''
  name: forceCommonLabels
  type: boolean
- description: ''
  name: ignoreMissingComponents
  type: boolean
- description: ''
  name: images
  type: array
- description: KubeVersion specifies the Kubernetes API version to pass to Helm when templating manifests. By default, Argo CD uses the Kubernetes version of the target cluster.
  name: kubeVersion
  type: string
- description: ''
  name: labelIncludeTemplates
  type: boolean
- description: ''
  name: labelWithoutSelector
  type: boolean
- description: ''
  name: namePrefix
  type: string
- description: ''
  name: nameSuffix
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: patches
  type: array
- description: ''
  name: replicas
  type: array
- description: ''
  name: version
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-source-kustomize-schema.json
slug: argo-cd-v1alpha1-application-source-kustomize
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSourceKustomize
---
