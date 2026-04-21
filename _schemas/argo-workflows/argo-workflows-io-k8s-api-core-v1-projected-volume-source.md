---
description: Represents a projected volume source
layout: schema
name: io.k8s.api.core.v1.ProjectedVolumeSource
properties_list:
- description: defaultMode are the mode bits used to set permissions on created files by default. Must be an octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts both octal and decima
  name: defaultMode
  type: integer
- description: sources is the list of volume projections. Each entry in this list handles one source.
  name: sources
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-projected-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-projected-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ProjectedVolumeSource
---
