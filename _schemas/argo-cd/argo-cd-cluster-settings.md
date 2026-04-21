---
description: clusterSettings schema from Argo CD API
layout: schema
name: clusterSettings
properties_list:
- description: ''
  name: additionalUrls
  type: array
- description: ''
  name: appLabelKey
  type: string
- description: ''
  name: appsInAnyNamespaceEnabled
  type: boolean
- description: 'Deprecated: use sidecar plugins instead.'
  name: configManagementPlugins
  type: array
- description: ''
  name: controllerNamespace
  type: string
- description: ''
  name: dexConfig
  type: object
- description: ''
  name: execEnabled
  type: boolean
- description: ''
  name: googleAnalytics
  type: object
- description: ''
  name: help
  type: object
- description: ''
  name: hydratorEnabled
  type: boolean
- description: ''
  name: impersonationEnabled
  type: boolean
- description: ''
  name: installationID
  type: string
- description: ''
  name: kustomizeOptions
  type: object
- description: ''
  name: kustomizeVersions
  type: array
- description: ''
  name: oidcConfig
  type: object
- description: ''
  name: passwordPattern
  type: string
- description: ''
  name: plugins
  type: array
- description: ''
  name: resourceOverrides
  type: object
- description: ''
  name: statusBadgeEnabled
  type: boolean
- description: ''
  name: statusBadgeRootUrl
  type: string
- description: ''
  name: syncWithReplaceAllowed
  type: boolean
- description: ''
  name: trackingMethod
  type: string
- description: ''
  name: uiBannerContent
  type: string
- description: ''
  name: uiBannerPermanent
  type: boolean
- description: ''
  name: uiBannerPosition
  type: string
- description: ''
  name: uiBannerURL
  type: string
- description: ''
  name: uiCssURL
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: userLoginsDisabled
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-cluster-settings-schema.json
slug: argo-cd-cluster-settings
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: clusterSettings
---
