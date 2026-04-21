---
description: A workflow artifact
layout: schema
name: Artifact
properties_list:
- description: ''
  name: name
  type: string
- description: Path in the container where artifact is placed
  name: path
  type: string
- description: Source artifact reference
  name: from
  type: string
- description: ''
  name: s3
  type: object
- description: ''
  name: git
  type: object
- description: ''
  name: http
  type: object
- description: ''
  name: archive
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-artifact-schema.json
slug: argo-workflows-artifact
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Artifact
---
