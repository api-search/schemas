---
description: SFTPEventSource describes an event-source for sftp related events.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SFTPEventSource
properties_list:
- description: Address sftp address.
  name: address
  type: object
- description: ''
  name: eventType
  type: string
- description: ''
  name: filter
  type: object
- description: ''
  name: metadata
  type: object
- description: Password required for authentication if any.
  name: password
  type: object
- description: ''
  name: pollIntervalDuration
  type: string
- description: SSHKeySecret refers to the secret that contains SSH key. Key needs to contain private key and public key.
  name: sshKeySecret
  type: object
- description: Username required for authentication if any.
  name: username
  type: object
- description: ''
  name: watchPathConfig
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sftp-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sftp-event-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SFTPEventSource
---
