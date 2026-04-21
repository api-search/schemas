---
description: Observed state and operational status of an Argo CD application.
layout: schema
name: ApplicationStatus
properties_list:
- description: Current sync status.
  name: sync
  type: object
- description: Current health status.
  name: health
  type: object
- description: State of the current or most recent operation.
  name: operationState
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-application-status-schema.json
slug: argo-cd-application-status
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ApplicationStatus
---
