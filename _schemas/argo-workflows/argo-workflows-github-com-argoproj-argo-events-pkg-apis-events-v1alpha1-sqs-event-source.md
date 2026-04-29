---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SQSEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SQSEventSource
properties_list:
- description: ''
  name: accessKey
  type: object
- description: ''
  name: dlq
  type: boolean
- description: ''
  name: endpoint
  type: string
- description: ''
  name: filter
  type: object
- description: ''
  name: jsonBody
  type: boolean
- description: ''
  name: metadata
  type: object
- description: ''
  name: queue
  type: string
- description: ''
  name: queueAccountId
  type: string
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
  name: sessionToken
  type: object
- description: WaitTimeSeconds is The duration (in seconds) for which the call waits for a message to arrive in the queue before returning.
  name: waitTimeSeconds
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sqs-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sqs-event-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sqs-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SQSEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SQSEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessKey\": {\n      \"title\": \"AccessKey refers K8s secret containing aws access key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"dlq\": {\n      \"type\": \"boolean\",\n      \"title\": \"DLQ specifies if a dead-letter queue is configured for messages that can't be processed successfully.\\nIf set to true, messages with invalid payload won't be acknowledged to allow to forward them farther\
  \ to the dead-letter queue.\\nThe default value is false.\\n+optional\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"title\": \"Endpoint configures connection to a specific SQS endpoint instead of Amazons servers\\n+optional\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"JSONBody specifies that all event body payload coming from this\\nsource will be JSON\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"queue\": {\n      \"type\": \"string\",\n      \"title\": \"Queue is AWS SQS queue to listen to for messages\"\n    },\n    \"\
  queueAccountId\": {\n      \"type\": \"string\",\n      \"title\": \"QueueAccountID is the ID of the account that created the queue to monitor\\n+optional\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"title\": \"Region is AWS region\"\n    },\n    \"roleARN\": {\n      \"type\": \"string\",\n      \"title\": \"RoleARN is the Amazon Resource Name (ARN) of the role to assume.\\n+optional\"\n    },\n    \"secretKey\": {\n      \"title\": \"SecretKey refers K8s secret containing aws secret key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"sessionToken\": {\n      \"title\": \"SessionToken refers to K8s secret containing AWS temporary credentials(STS) session token\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"waitTimeSeconds\": {\n      \"description\": \"WaitTimeSeconds is The duration (in seconds) for which the call waits for a message to arrive\\nin the queue before returning.\"\
  ,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-sqs-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SQSEventSource
---
