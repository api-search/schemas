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
source_filename: argo-workflows-io-k8s-api-core-v1-pod-certificate-projection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-pod-certificate-projection-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PodCertificateProjection\",\n  \"description\": \"PodCertificateProjection provides a private key and X.509 certificate in the pod filesystem.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateChainPath\": {\n      \"description\": \"Write the certificate chain at this path in the projected volume.\\n\\nMost applications should use credentialBundlePath.  When using keyPath and certificateChainPath, your application needs to check that the key and leaf certificate are consistent, because it is possible to read the files mid-rotation.\",\n      \"type\": \"string\"\n    },\n    \"credentialBundlePath\": {\n      \"description\": \"Write the credential bundle at this path in the projected\
  \ volume.\\n\\nThe credential bundle is a single file that contains multiple PEM blocks. The first PEM block is a PRIVATE KEY block, containing a PKCS#8 private key.\\n\\nThe remaining blocks are CERTIFICATE blocks, containing the issued certificate chain from the signer (leaf and any intermediates).\\n\\nUsing credentialBundlePath lets your Pod's application code make a single atomic read that retrieves a consistent key and certificate chain.  If you project them to separate files, your application code will need to additionally check that the leaf certificate was issued to the key.\",\n      \"type\": \"string\"\n    },\n    \"keyPath\": {\n      \"description\": \"Write the key at this path in the projected volume.\\n\\nMost applications should use credentialBundlePath.  When using keyPath and certificateChainPath, your application needs to check that the key and leaf certificate are consistent, because it is possible to read the files mid-rotation.\",\n      \"type\": \"string\"\n\
  \    },\n    \"keyType\": {\n      \"description\": \"The type of keypair Kubelet will generate for the pod.\\n\\nValid values are \\\"RSA3072\\\", \\\"RSA4096\\\", \\\"ECDSAP256\\\", \\\"ECDSAP384\\\", \\\"ECDSAP521\\\", and \\\"ED25519\\\".\",\n      \"type\": \"string\"\n    },\n    \"maxExpirationSeconds\": {\n      \"description\": \"maxExpirationSeconds is the maximum lifetime permitted for the certificate.\\n\\nKubelet copies this value verbatim into the PodCertificateRequests it generates for this projection.\\n\\nIf omitted, kube-apiserver will set it to 86400(24 hours). kube-apiserver will reject values shorter than 3600 (1 hour).  The maximum allowable value is 7862400 (91 days).\\n\\nThe signer implementation is then free to issue a certificate with any lifetime *shorter* than MaxExpirationSeconds, but no shorter than 3600 seconds (1 hour).  This constraint is enforced by kube-apiserver. `kubernetes.io` signers will never issue certificates with a lifetime longer than 24 hours.\"\
  ,\n      \"type\": \"integer\"\n    },\n    \"signerName\": {\n      \"description\": \"Kubelet's generated CSRs will be addressed to this signer.\",\n      \"type\": \"string\"\n    },\n    \"userAnnotations\": {\n      \"description\": \"userAnnotations allow pod authors to pass additional information to the signer implementation.  Kubernetes does not restrict or validate this metadata in any way.\\n\\nThese values are copied verbatim into the `spec.unverifiedUserAnnotations` field of the PodCertificateRequest objects that Kubelet creates.\\n\\nEntries are subject to the same validation as object metadata annotations, with the addition that all keys must be domain-prefixed. No restrictions are placed on values, except an overall size limitation on the entire field.\\n\\nSigners should document the keys and values they support. Signers should deny requests that contain keys they do not recognize.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"\
  string\"\n      }\n    }\n  },\n  \"required\": [\n    \"signerName\",\n    \"keyType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-pod-certificate-projection-schema.json
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
