---
description: Target Kubernetes cluster and namespace for application deployment.
layout: schema
name: ApplicationDestination
properties_list:
- description: Kubernetes API server URL of the target cluster. Use https://kubernetes.default.svc for the in-cluster target.
  name: server
  type: string
- description: Name of the registered cluster. Mutually exclusive with server.
  name: name
  type: string
- description: Target namespace in the destination cluster.
  name: namespace
  type: string
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-application-destination-schema.json
slug: argo-cd-application-destination
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ApplicationDestination
---
