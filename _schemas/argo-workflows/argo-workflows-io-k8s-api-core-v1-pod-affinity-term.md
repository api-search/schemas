---
description: Defines a set of pods (namely those matching the labelSelector relative to the given namespace(s)) that this pod should be co-located (affinity) or not co-located (anti-affinity) with, where co-located is defined as running on a node whose value of the label with key <topologyKey> matches that of any node on which a pod of the set of pods is running
layout: schema
name: io.k8s.api.core.v1.PodAffinityTerm
properties_list:
- description: A label query over a set of resources, in this case pods. If it's null, this PodAffinityTerm matches with no Pods.
  name: labelSelector
  type: object
- description: MatchLabelKeys is a set of pod label keys to select which pods will be taken into consideration. The keys are used to lookup values from the incoming pod labels, those key-value labels are merged with
  name: matchLabelKeys
  type: array
- description: MismatchLabelKeys is a set of pod label keys to select which pods will be taken into consideration. The keys are used to lookup values from the incoming pod labels, those key-value labels are merged w
  name: mismatchLabelKeys
  type: array
- description: 'A label query over the set of namespaces that the term applies to. The term is applied to the union of the namespaces selected by this field and the ones listed in the namespaces field. null selector '
  name: namespaceSelector
  type: object
- description: namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null
  name: namespaces
  type: array
- description: 'This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching the labelSelector in the specified namespaces, where co-located is defined as running on a node whose '
  name: topologyKey
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-pod-affinity-term-schema.json
slug: argo-workflows-io-k8s-api-core-v1-pod-affinity-term
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PodAffinityTerm
---
