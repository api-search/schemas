---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPQueueDeclareConfig schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPQueueDeclareConfig
properties_list:
- description: ''
  name: arguments
  type: string
- description: ''
  name: autoDelete
  type: boolean
- description: ''
  name: durable
  type: boolean
- description: ''
  name: exclusive
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: noWait
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-queue-declare-config-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-queue-declare-config
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-queue-declare-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-queue-declare-config-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPQueueDeclareConfig\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPQueueDeclareConfig schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arguments\": {\n      \"type\": \"string\",\n      \"title\": \"Arguments of a queue (also known as \\\"x-arguments\\\") used for optional features and plugins\\n+optional\"\n    },\n    \"autoDelete\": {\n      \"type\": \"boolean\",\n      \"title\": \"AutoDelete removes the queue when no consumers are active\\n+optional\"\n    },\n    \"durable\": {\n      \"type\": \"boolean\",\n      \"title\": \"Durable\
  \ keeps the queue also after the server restarts\\n+optional\"\n    },\n    \"exclusive\": {\n      \"type\": \"boolean\",\n      \"title\": \"Exclusive sets the queues to be accessible only by the connection that declares them and will be\\ndeleted wgen the connection closes\\n+optional\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name of the queue. If empty the server auto-generates a unique name for this queue\\n+optional\"\n    },\n    \"noWait\": {\n      \"type\": \"boolean\",\n      \"title\": \"NowWait when true, the queue assumes to be declared on the server\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-queue-declare-config-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPQueueDeclareConfig
---
