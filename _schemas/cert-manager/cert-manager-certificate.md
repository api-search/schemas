---
description: JSON Schema for the cert-manager Certificate custom resource (cert-manager.io/v1). A Certificate is a Kubernetes CRD that declaratively specifies a desired X.509 certificate, including the secret name where it will be stored, the issuer that should sign it, the DNS names and other SANs to include, and renewal configuration. cert-manager controllers watch Certificate resources and automatically obtain, renew, and store the resulting TLS key pairs.
layout: schema
name: cert-manager Certificate
properties_list:
- description: The cert-manager API version for this resource.
  name: apiVersion
  type: string
- description: The resource kind, always Certificate.
  name: kind
  type: string
- description: Kubernetes ObjectMeta for the Certificate resource including name and namespace.
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
schema_file: json-schema/cert-manager-certificate-schema.json
slug: cert-manager-certificate
tags:
- Certificates
- Cloud Native
- Graduated
- Kubernetes
- Security
- TLS
title: cert-manager Certificate
---
