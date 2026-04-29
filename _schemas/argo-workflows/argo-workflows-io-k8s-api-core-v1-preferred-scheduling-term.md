---
description: An empty preferred scheduling term matches all objects with implicit weight 0 (i.e. it's a no-op). A null preferred scheduling term matches no objects (i.e. is also a no-op).
layout: schema
name: io.k8s.api.core.v1.PreferredSchedulingTerm
properties_list:
- description: A node selector term, associated with the corresponding weight.
  name: preference
  type: object
- description: Weight associated with matching the corresponding nodeSelectorTerm, in the range 1-100.
  name: weight
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-preferred-scheduling-term-schema.json
slug: argo-workflows-io-k8s-api-core-v1-preferred-scheduling-term
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-preferred-scheduling-term-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PreferredSchedulingTerm\",\n  \"description\": \"An empty preferred scheduling term matches all objects with implicit weight 0 (i.e. it's a no-op). A null preferred scheduling term matches no objects (i.e. is also a no-op).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"preference\": {\n      \"description\": \"A node selector term, associated with the corresponding weight.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.NodeSelectorTerm\"\n    },\n    \"weight\": {\n      \"description\": \"Weight associated with matching the corresponding nodeSelectorTerm, in the range 1-100.\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"weight\",\n    \"preference\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-preferred-scheduling-term-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PreferredSchedulingTerm
---
