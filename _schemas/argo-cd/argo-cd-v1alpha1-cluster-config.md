---
description: ClusterConfig is the configuration attributes. This structure is subset of the go-client rest.Config with annotations added for marshalling.
layout: schema
name: v1alpha1ClusterConfig
properties_list:
- description: ''
  name: awsAuthConfig
  type: object
- description: 'Server requires Bearer authentication. This client will not attempt to use refresh tokens for an OAuth2 flow. TODO: demonstrate an OAuth2 compatible client.'
  name: bearerToken
  type: string
- description: DisableCompression bypasses automatic GZip compression requests to the server.
  name: disableCompression
  type: boolean
- description: ''
  name: execProviderConfig
  type: object
- description: ''
  name: password
  type: string
- description: ''
  name: proxyUrl
  type: string
- description: ''
  name: tlsClientConfig
  type: object
- description: ''
  name: username
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-cluster-config-schema.json
slug: argo-cd-v1alpha1-cluster-config
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ClusterConfig
---
