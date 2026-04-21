---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitlabEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitlabEventSource
properties_list:
- description: ''
  name: accessToken
  type: object
- description: ''
  name: deleteHookOnFinish
  type: boolean
- description: ''
  name: enableSSLVerification
  type: boolean
- description: Events are gitlab event to listen to. Refer https://github.com/xanzy/go-gitlab/blob/bf34eca5d13a9f4c3f501d8a97b8ac226d55e4d9/projects.go#L794.
  name: events
  type: array
- description: ''
  name: filter
  type: object
- description: ''
  name: gitlabBaseURL
  type: string
- description: ''
  name: groups
  type: array
- description: ''
  name: metadata
  type: object
- description: ''
  name: projectID
  type: string
- description: ''
  name: projects
  type: array
- description: ''
  name: secretToken
  type: object
- description: ''
  name: webhook
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gitlab-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-gitlab-event-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitlabEventSource
---
