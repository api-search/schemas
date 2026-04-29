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
source_filename: argo-workflows-io-k8s-api-core-v1-pod-affinity-term-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-pod-affinity-term-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PodAffinityTerm\",\n  \"description\": \"Defines a set of pods (namely those matching the labelSelector relative to the given namespace(s)) that this pod should be co-located (affinity) or not co-located (anti-affinity) with, where co-located is defined as running on a node whose value of the label with key <topologyKey> matches that of any node on which a pod of the set of pods is running\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"labelSelector\": {\n      \"description\": \"A label query over a set of resources, in this case pods. If it's null, this PodAffinityTerm matches with no Pods.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelector\"\n    },\n    \"\
  matchLabelKeys\": {\n      \"description\": \"MatchLabelKeys is a set of pod label keys to select which pods will be taken into consideration. The keys are used to lookup values from the incoming pod labels, those key-value labels are merged with `labelSelector` as `key in (value)` to select the group of existing pods which pods will be taken into consideration for the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming pod labels will be ignored. The default value is empty. The same key is forbidden to exist in both matchLabelKeys and labelSelector. Also, matchLabelKeys cannot be set when labelSelector isn't set.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"mismatchLabelKeys\": {\n      \"description\": \"MismatchLabelKeys is a set of pod label keys to select which pods will be taken into consideration. The keys are used to lookup values from the incoming pod\
  \ labels, those key-value labels are merged with `labelSelector` as `key notin (value)` to select the group of existing pods which pods will be taken into consideration for the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming pod labels will be ignored. The default value is empty. The same key is forbidden to exist in both mismatchLabelKeys and labelSelector. Also, mismatchLabelKeys cannot be set when labelSelector isn't set.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"namespaceSelector\": {\n      \"description\": \"A label query over the set of namespaces that the term applies to. The term is applied to the union of the namespaces selected by this field and the ones listed in the namespaces field. null selector and null or empty namespaces list means \\\"this pod's namespace\\\". An empty selector ({}) matches all namespaces.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelector\"\
  \n    },\n    \"namespaces\": {\n      \"description\": \"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \\\"this pod's namespace\\\".\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"topologyKey\": {\n      \"description\": \"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching the labelSelector in the specified namespaces, where co-located is defined as running on a node whose value of the label with key topologyKey matches that of any node on which any of the selected pods is running. Empty topologyKey is not allowed.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"topologyKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-pod-affinity-term-schema.json
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
