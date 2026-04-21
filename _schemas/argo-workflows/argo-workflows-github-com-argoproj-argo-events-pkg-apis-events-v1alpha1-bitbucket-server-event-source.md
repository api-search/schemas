---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketServerEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketServerEventSource
properties_list:
- description: ''
  name: accessToken
  type: object
- description: BitbucketServerBaseURL is the base URL for API requests to a custom endpoint.
  name: bitbucketserverBaseURL
  type: string
- description: ''
  name: checkInterval
  type: string
- description: ''
  name: deleteHookOnFinish
  type: boolean
- description: ''
  name: events
  type: array
- description: ''
  name: filter
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: oneEventPerChange
  type: boolean
- description: ''
  name: projectKey
  type: string
- description: ''
  name: projects
  type: array
- description: ''
  name: repositories
  type: array
- description: ''
  name: repositorySlug
  type: string
- description: ''
  name: skipBranchRefsChangedOnOpenPR
  type: boolean
- description: ''
  name: tls
  type: object
- description: Webhook holds configuration to run a http server.
  name: webhook
  type: object
- description: ''
  name: webhookSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-server-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-bitbucket-server-event-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketServerEventSource
---
