---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AWSLambdaTrigger schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AWSLambdaTrigger
properties_list:
- description: ''
  name: accessKey
  type: object
- description: FunctionName refers to the name of the function to invoke.
  name: functionName
  type: string
- description: Choose from the following options. * RequestResponse (default) - Invoke the function synchronously. Keep the connection open until the function returns a response or times out. The API response includ
  name: invocationType
  type: string
- description: ''
  name: parameters
  type: array
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: ''
  name: region
  type: string
- description: ''
  name: roleARN
  type: string
- description: ''
  name: secretKey
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-aws-lambda-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-aws-lambda-trigger
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AWSLambdaTrigger
---
