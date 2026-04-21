---
description: ResourceDiff holds the diff between a live and target resource object in Argo CD. It is used to compare the desired state (from Git/Helm) with the actual state in the cluster.
layout: schema
name: v1alpha1ResourceDiff
properties_list:
- description: 'Diff contains the JSON patch representing the difference between the live and target resource. Deprecated: Use NormalizedLiveState and PredictedLiveState instead to compute differences.'
  name: diff
  type: string
- description: Group represents the API group of the resource (e.g., "apps" for Deployments).
  name: group
  type: string
- description: Hook indicates whether this resource is a hook resource (e.g., pre-sync or post-sync hooks).
  name: hook
  type: boolean
- description: Kind represents the Kubernetes resource kind (e.g., "Deployment", "Service").
  name: kind
  type: string
- description: LiveState contains the JSON-serialized resource manifest of the resource currently running in the cluster.
  name: liveState
  type: string
- description: Modified indicates whether the live resource has changes compared to the target resource.
  name: modified
  type: boolean
- description: Name is the name of the resource.
  name: name
  type: string
- description: Namespace specifies the namespace where the resource exists.
  name: namespace
  type: string
- description: NormalizedLiveState contains the JSON-serialized live resource state after applying normalizations. Normalizations may include ignoring irrelevant fields like timestamps or defaults applied by Kuberne
  name: normalizedLiveState
  type: string
- description: PredictedLiveState contains the JSON-serialized resource state that Argo CD predicts based on the combination of the normalized live state and the desired target state.
  name: predictedLiveState
  type: string
- description: ResourceVersion is the Kubernetes resource version, which helps in tracking changes.
  name: resourceVersion
  type: string
- description: TargetState contains the JSON-serialized resource manifest as defined in the Git/Helm repository.
  name: targetState
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-diff-schema.json
slug: argo-cd-v1alpha1-resource-diff
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceDiff
---
