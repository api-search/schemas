---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SNSEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SNSEventSource
properties_list:
- description: ''
  name: accessKey
  type: object
- description: ''
  name: endpoint
  type: string
- description: ''
  name: filter
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: region
  type: string
- description: ''
  name: roleARN
  type: string
- description: ''
  name: secretKey
  type: object
- description: ''
  name: topicArn
  type: string
- description: ''
  name: validateSignature
  type: boolean
- description: ''
  name: webhook
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sns-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sns-event-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sns-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SNSEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SNSEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessKey\": {\n      \"title\": \"AccessKey refers K8s secret containing aws access key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"title\": \"Endpoint configures connection to a specific SNS endpoint instead of Amazons servers\\n+optional\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\
  \n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"title\": \"Region is AWS region\"\n    },\n    \"roleARN\": {\n      \"type\": \"string\",\n      \"title\": \"RoleARN is the Amazon Resource Name (ARN) of the role to assume.\\n+optional\"\n    },\n    \"secretKey\": {\n      \"title\": \"SecretKey refers K8s secret containing aws secret key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"topicArn\": {\n      \"type\": \"string\",\n      \"title\": \"TopicArn\"\n    },\n    \"validateSignature\": {\n      \"type\": \"boolean\",\n      \"title\": \"ValidateSignature is boolean that can be set to true for SNS signature verification\\n+optional\"\n    },\n    \"webhook\": {\n      \"title\"\
  : \"Webhook configuration for http server\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sns-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SNSEventSource
---
