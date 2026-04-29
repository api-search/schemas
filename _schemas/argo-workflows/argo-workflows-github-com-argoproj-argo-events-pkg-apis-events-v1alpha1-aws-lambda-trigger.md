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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-aws-lambda-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AWSLambdaTrigger\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AWSLambdaTrigger schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessKey\": {\n      \"title\": \"AccessKey refers K8s secret containing aws access key\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"functionName\": {\n      \"description\": \"FunctionName refers to the name of the function to invoke.\",\n      \"type\": \"string\"\n    },\n    \"invocationType\": {\n      \"description\": \"Choose from the following options.\\n\\n   * RequestResponse\
  \ (default) - Invoke the function synchronously. Keep\\n   the connection open until the function returns a response or times out.\\n   The API response includes the function response and additional data.\\n\\n   * Event - Invoke the function asynchronously. Send events that fail multiple\\n   times to the function's dead-letter queue (if it's configured). The API\\n   response only includes a status code.\\n\\n   * DryRun - Validate parameter values and verify that the user or role\\n   has permission to invoke the function.\\n+optional\",\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"title\": \"Parameters is the list of key-value extracted from event's payload that are applied to\\nthe trigger resource.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"payload\": {\n      \"description\": \"Payload is the list of key-value\
  \ extracted from an event payload to construct the request payload.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"title\": \"Region is AWS region\"\n    },\n    \"roleARN\": {\n      \"type\": \"string\",\n      \"title\": \"RoleARN is the Amazon Resource Name (ARN) of the role to assume.\\n+optional\"\n    },\n    \"secretKey\": {\n      \"title\": \"SecretKey refers K8s secret containing aws secret key\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-aws-lambda-trigger-schema.json
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
