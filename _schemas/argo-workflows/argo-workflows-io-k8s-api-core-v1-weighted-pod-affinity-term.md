---
description: The weights of all of the matched WeightedPodAffinityTerm fields are added per-node to find the most preferred node(s)
layout: schema
name: io.k8s.api.core.v1.WeightedPodAffinityTerm
properties_list:
- description: Required. A pod affinity term, associated with the corresponding weight.
  name: podAffinityTerm
  type: object
- description: weight associated with matching the corresponding podAffinityTerm, in the range 1-100.
  name: weight
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-weighted-pod-affinity-term-schema.json
slug: argo-workflows-io-k8s-api-core-v1-weighted-pod-affinity-term
source_filename: argo-workflows-io-k8s-api-core-v1-weighted-pod-affinity-term-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-weighted-pod-affinity-term-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.WeightedPodAffinityTerm\",\n  \"description\": \"The weights of all of the matched WeightedPodAffinityTerm fields are added per-node to find the most preferred node(s)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"podAffinityTerm\": {\n      \"description\": \"Required. A pod affinity term, associated with the corresponding weight.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PodAffinityTerm\"\n    },\n    \"weight\": {\n      \"description\": \"weight associated with matching the corresponding podAffinityTerm, in the range 1-100.\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"weight\",\n    \"podAffinityTerm\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-weighted-pod-affinity-term-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.WeightedPodAffinityTerm
---
