---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GithubEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GithubEventSource
properties_list:
- description: ''
  name: active
  type: boolean
- description: ''
  name: apiToken
  type: object
- description: ''
  name: contentType
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
  name: githubApp
  type: object
- description: ''
  name: githubBaseURL
  type: string
- description: ''
  name: githubUploadURL
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: insecure
  type: boolean
- description: ''
  name: metadata
  type: object
- description: Organizations holds the names of organizations (used for organization level webhooks). Not required if Repositories is set.
  name: organizations
  type: array
- description: ''
  name: owner
  type: string
- description: Repositories holds the information of repositories, which uses repo owner as the key, and list of repo names as the value. Not required if Organizations is set.
  name: repositories
  type: array
- description: ''
  name: repository
  type: string
- description: ''
  name: webhook
  type: object
- description: ''
  name: webhookSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-github-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-github-event-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GithubEventSource
---
