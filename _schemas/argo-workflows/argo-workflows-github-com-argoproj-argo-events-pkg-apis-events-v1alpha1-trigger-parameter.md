---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter
properties_list:
- description: Dest is the JSONPath of a resource key. A path is a series of keys separated by a dot. The colon character can be escaped with '.' The -1 key can be used to append a value to an existing array. See ht
  name: dest
  type: string
- description: Operation is what to do with the existing value at Dest, whether to 'prepend', 'overwrite', or 'append' it.
  name: operation
  type: string
- description: ''
  name: src
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter
---
