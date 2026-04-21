---
description: v1alpha1TLSClientConfig schema from Argo CD API
layout: schema
name: v1alpha1TLSClientConfig
properties_list:
- description: ''
  name: caData
  type: string
- description: ''
  name: certData
  type: string
- description: Insecure specifies that the server should be accessed without verifying the TLS certificate. For testing only.
  name: insecure
  type: boolean
- description: ''
  name: keyData
  type: string
- description: ServerName is passed to the server for SNI and is used in the client to check server certificates against. If ServerName is empty, the hostname used to contact the server is used.
  name: serverName
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-tls-client-config-schema.json
slug: argo-cd-v1alpha1-tls-client-config
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1TLSClientConfig
---
