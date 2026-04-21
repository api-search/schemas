---
description: A registered Git or Helm chart repository.
layout: schema
name: Repository
properties_list:
- description: Repository URL.
  name: repo
  type: string
- description: Repository type.
  name: type
  type: string
- description: Human-readable repository name.
  name: name
  type: string
- description: Current connection status.
  name: connectionState
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-repository-schema.json
slug: argo-cd-repository
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Repository
---
