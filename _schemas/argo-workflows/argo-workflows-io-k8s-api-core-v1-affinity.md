---
description: Affinity is a group of affinity scheduling rules.
layout: schema
name: io.k8s.api.core.v1.Affinity
properties_list:
- description: Describes node affinity scheduling rules for the pod.
  name: nodeAffinity
  type: object
- description: Describes pod affinity scheduling rules (e.g. co-locate this pod in the same node, zone, etc. as some other pod(s)).
  name: podAffinity
  type: object
- description: Describes pod anti-affinity scheduling rules (e.g. avoid putting this pod in the same node, zone, etc. as some other pod(s)).
  name: podAntiAffinity
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-affinity-schema.json
slug: argo-workflows-io-k8s-api-core-v1-affinity
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.Affinity
---
