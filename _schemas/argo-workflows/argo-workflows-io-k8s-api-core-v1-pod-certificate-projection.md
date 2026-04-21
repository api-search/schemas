---
description: PodCertificateProjection provides a private key and X.509 certificate in the pod filesystem.
layout: schema
name: io.k8s.api.core.v1.PodCertificateProjection
properties_list:
- description: Write the certificate chain at this path in the projected volume. Most applications should use credentialBundlePath. When using keyPath and certificateChainPath, your application needs to check that t
  name: certificateChainPath
  type: string
- description: Write the credential bundle at this path in the projected volume. The credential bundle is a single file that contains multiple PEM blocks. The first PEM block is a PRIVATE KEY block, containing a PKC
  name: credentialBundlePath
  type: string
- description: Write the key at this path in the projected volume. Most applications should use credentialBundlePath. When using keyPath and certificateChainPath, your application needs to check that the key and lea
  name: keyPath
  type: string
- description: The type of keypair Kubelet will generate for the pod. Valid values are "RSA3072", "RSA4096", "ECDSAP256", "ECDSAP384", "ECDSAP521", and "ED25519".
  name: keyType
  type: string
- description: maxExpirationSeconds is the maximum lifetime permitted for the certificate. Kubelet copies this value verbatim into the PodCertificateRequests it generates for this projection. If omitted, kube-apiser
  name: maxExpirationSeconds
  type: integer
- description: Kubelet's generated CSRs will be addressed to this signer.
  name: signerName
  type: string
- description: 'userAnnotations allow pod authors to pass additional information to the signer implementation. Kubernetes does not restrict or validate this metadata in any way. These values are copied verbatim into '
  name: userAnnotations
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-pod-certificate-projection-schema.json
slug: argo-workflows-io-k8s-api-core-v1-pod-certificate-projection
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PodCertificateProjection
---
