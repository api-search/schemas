---
description: Projection that may be projected along with other supported volume types. Exactly one of these fields must be set.
layout: schema
name: io.k8s.api.core.v1.VolumeProjection
properties_list:
- description: ClusterTrustBundle allows a pod to access the `.spec.trustBundle` field of ClusterTrustBundle objects in an auto-updating file. Alpha, gated by the ClusterTrustBundleProjection feature gate. ClusterTr
  name: clusterTrustBundle
  type: object
- description: configMap information about the configMap data to project
  name: configMap
  type: object
- description: downwardAPI information about the downwardAPI data to project
  name: downwardAPI
  type: object
- description: Projects an auto-rotating credential bundle (private key and certificate chain) that the pod can use either as a TLS client or server. Kubelet generates a private key and uses it to send a PodCertific
  name: podCertificate
  type: object
- description: secret information about the secret data to project
  name: secret
  type: object
- description: serviceAccountToken is information about the serviceAccountToken data to project
  name: serviceAccountToken
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-volume-projection-schema.json
slug: argo-workflows-io-k8s-api-core-v1-volume-projection
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.VolumeProjection
---
