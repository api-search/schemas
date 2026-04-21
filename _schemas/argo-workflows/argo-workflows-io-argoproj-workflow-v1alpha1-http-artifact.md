---
description: HTTPArtifact allows a file served on HTTP to be placed as an input artifact in a container
layout: schema
name: io.argoproj.workflow.v1alpha1.HTTPArtifact
properties_list:
- description: Auth contains information for client authentication
  name: auth
  type: object
- description: Headers are an optional list of headers to send with HTTP requests for artifacts
  name: headers
  type: array
- description: URL of the artifact
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-http-artifact
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.HTTPArtifact
---
