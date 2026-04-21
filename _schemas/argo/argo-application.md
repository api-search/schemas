---
description: JSON Schema for the Argo CD Application resource specification, defining the structure of GitOps application definitions for Kubernetes declarative continuous delivery.
layout: schema
name: Argo CD Application Spec
properties_list:
- description: API version for Argo CD resources
  name: apiVersion
  type: string
- description: Kind of the Argo CD resource
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-application-schema.json
slug: argo-application
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Argo CD Application Spec
---
