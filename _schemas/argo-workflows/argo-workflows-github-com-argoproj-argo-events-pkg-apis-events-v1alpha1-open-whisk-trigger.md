---
description: OpenWhiskTrigger refers to the specification of the OpenWhisk trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.OpenWhiskTrigger
properties_list:
- description: Name of the action/function.
  name: actionName
  type: string
- description: ''
  name: authToken
  type: object
- description: Host URL of the OpenWhisk.
  name: host
  type: string
- description: Namespace for the action. Defaults to "_". +optional.
  name: namespace
  type: string
- description: ''
  name: parameters
  type: array
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: ''
  name: version
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-open-whisk-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-open-whisk-trigger
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.OpenWhiskTrigger
---
