---
description: JSON Schema for cert-manager Issuer and ClusterIssuer custom resources (cert-manager.io/v1). An Issuer represents a certificate authority scoped to a single namespace, while a ClusterIssuer is cluster-scoped and can serve Certificate resources across all namespaces. Both resources configure the backend certificate authority connection including ACME, CA, SelfSigned, Vault, and Venafi issuer types.
layout: schema
name: cert-manager Issuer and ClusterIssuer
properties_list:
- description: The cert-manager API version.
  name: apiVersion
  type: string
- description: 'The resource kind: Issuer (namespace-scoped) or ClusterIssuer (cluster-scoped).'
  name: kind
  type: string
- description: Kubernetes ObjectMeta for the Issuer or ClusterIssuer resource.
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
provider_name: Cert-Manager
provider_slug: cert-manager
schema_file: json-schema/cert-manager-issuer-schema.json
slug: cert-manager-issuer
tags:
- Certificates
- Cloud Native
- Graduated
- Kubernetes
- Security
- TLS
title: cert-manager Issuer and ClusterIssuer
---
