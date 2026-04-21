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
