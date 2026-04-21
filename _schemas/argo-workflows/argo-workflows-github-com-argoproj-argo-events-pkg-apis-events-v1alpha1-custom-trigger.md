---
description: CustomTrigger refers to the specification of the custom trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CustomTrigger
properties_list:
- description: CertSecret refers to the secret that contains cert for secure connection between sensor and custom trigger gRPC server.
  name: certSecret
  type: object
- description: Parameters is the list of parameters that is applied to resolved custom trigger trigger object.
  name: parameters
  type: array
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: ''
  name: secure
  type: boolean
- description: ServerNameOverride for the secure connection between sensor and custom trigger gRPC server.
  name: serverNameOverride
  type: string
- description: ''
  name: serverURL
  type: string
- description: Spec is the custom trigger resource specification that custom trigger gRPC server knows how to interpret.
  name: spec
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-custom-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-custom-trigger
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CustomTrigger
---
