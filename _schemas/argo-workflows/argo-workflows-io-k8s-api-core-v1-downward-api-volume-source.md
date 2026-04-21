---
description: DownwardAPIVolumeSource represents a volume containing downward API info. Downward API volumes support ownership management and SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.DownwardAPIVolumeSource
properties_list:
- description: 'Optional: mode bits to use on created files by default. Must be a Optional: mode bits used to set permissions on created files by default. Must be an octal value between 0000 and 0777 or a decimal val'
  name: defaultMode
  type: integer
- description: Items is a list of downward API volume file
  name: items
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-downward-api-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-downward-api-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.DownwardAPIVolumeSource
---
