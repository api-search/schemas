---
description: SlackTrigger refers to the specification of the slack notification trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SlackTrigger
properties_list:
- description: ''
  name: attachments
  type: string
- description: ''
  name: blocks
  type: string
- description: ''
  name: channel
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: sender
  type: object
- description: SlackToken refers to the Kubernetes secret that holds the slack token required to send messages.
  name: slackToken
  type: object
- description: ''
  name: thread
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-slack-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-slack-trigger
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SlackTrigger
---
