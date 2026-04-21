---
description: Desired state specification for an Argo CD application.
layout: schema
name: ApplicationSpec
properties_list:
- description: ''
  name: source
  type: object
- description: ''
  name: destination
  type: object
- description: Argo CD project this application belongs to.
  name: project
  type: string
- description: ''
  name: syncPolicy
  type: object
- description: Resource fields to ignore when computing sync status.
  name: ignoreDifferences
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-application-spec-schema.json
slug: argo-cd-application-spec
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ApplicationSpec
---
