---
description: ClusterTrustBundleProjection describes how to select a set of ClusterTrustBundle objects and project their contents into the pod filesystem.
layout: schema
name: io.k8s.api.core.v1.ClusterTrustBundleProjection
properties_list:
- description: Select all ClusterTrustBundles that match this label selector. Only has effect if signerName is set. Mutually-exclusive with name. If unset, interpreted as "match nothing". If set but empty, interpret
  name: labelSelector
  type: object
- description: Select a single ClusterTrustBundle by object name. Mutually-exclusive with signerName and labelSelector.
  name: name
  type: string
- description: If true, don't block pod startup if the referenced ClusterTrustBundle(s) aren't available. If using name, then the named ClusterTrustBundle is allowed not to exist. If using signerName, then the combi
  name: optional
  type: boolean
- description: Relative path from the volume root to write the bundle.
  name: path
  type: string
- description: Select all ClusterTrustBundles that match this signer name. Mutually-exclusive with name. The contents of all selected ClusterTrustBundles will be unified and deduplicated.
  name: signerName
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-cluster-trust-bundle-projection-schema.json
slug: argo-workflows-io-k8s-api-core-v1-cluster-trust-bundle-projection
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ClusterTrustBundleProjection
---
