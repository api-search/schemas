---
description: v1alpha1ApplicationSourceHelm schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSourceHelm
properties_list:
- description: APIVersions specifies the Kubernetes resource API versions to pass to Helm when templating manifests. By default, Argo CD uses the API versions of the target cluster. The format is [group/]version/kin
  name: apiVersions
  type: array
- description: ''
  name: fileParameters
  type: array
- description: ''
  name: ignoreMissingValueFiles
  type: boolean
- description: KubeVersion specifies the Kubernetes API version to pass to Helm when templating manifests. By default, Argo CD uses the Kubernetes version of the target cluster.
  name: kubeVersion
  type: string
- description: Namespace is an optional namespace to template with. If left empty, defaults to the app's destination namespace.
  name: namespace
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: passCredentials
  type: boolean
- description: ''
  name: releaseName
  type: string
- description: ''
  name: skipCrds
  type: boolean
- description: ''
  name: skipSchemaValidation
  type: boolean
- description: SkipTests skips test manifest installation step (Helm's --skip-tests).
  name: skipTests
  type: boolean
- description: ''
  name: valueFiles
  type: array
- description: ''
  name: values
  type: string
- description: ''
  name: valuesObject
  type: object
- description: ''
  name: version
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-source-helm-schema.json
slug: argo-cd-v1alpha1-application-source-helm
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSourceHelm
---
