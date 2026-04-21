---
description: io.argoproj.workflow.v1alpha1.HTTP schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.HTTP
properties_list:
- description: Body is content of the HTTP Request
  name: body
  type: string
- description: BodyFrom is content of the HTTP Request as Bytes
  name: bodyFrom
  type: object
- description: Headers are an optional list of headers to send with HTTP requests
  name: headers
  type: array
- description: InsecureSkipVerify is a bool when if set to true will skip TLS verification for the HTTP client
  name: insecureSkipVerify
  type: boolean
- description: Method is HTTP methods for HTTP Request
  name: method
  type: string
- description: SuccessCondition is an expression if evaluated to true is considered successful
  name: successCondition
  type: string
- description: TimeoutSeconds is request timeout for HTTP Request. Default is 30 seconds
  name: timeoutSeconds
  type: integer
- description: URL of the HTTP Request
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-http-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-http
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.HTTP
---
