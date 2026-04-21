---
description: A registered Kubernetes cluster deployment target.
layout: schema
name: Cluster
properties_list:
- description: Kubernetes API server URL.
  name: server
  type: string
- description: Cluster display name.
  name: name
  type: string
- description: Cluster connection configuration.
  name: config
  type: object
- description: Cluster information.
  name: info
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-cluster-schema.json
slug: argo-cd-cluster
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Cluster
---
