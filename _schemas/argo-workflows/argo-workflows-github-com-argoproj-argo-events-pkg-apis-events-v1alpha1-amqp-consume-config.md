---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPConsumeConfig schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPConsumeConfig
properties_list:
- description: ''
  name: autoAck
  type: boolean
- description: ''
  name: consumerTag
  type: string
- description: ''
  name: exclusive
  type: boolean
- description: ''
  name: noLocal
  type: boolean
- description: ''
  name: noWait
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-consume-config-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-consume-config
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-consume-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-consume-config-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPConsumeConfig\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPConsumeConfig schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autoAck\": {\n      \"type\": \"boolean\",\n      \"title\": \"AutoAck when true, the server will acknowledge deliveries to this consumer prior to writing\\nthe delivery to the network\\n+optional\"\n    },\n    \"consumerTag\": {\n      \"type\": \"string\",\n      \"title\": \"ConsumerTag is the identity of the consumer included in every delivery\\n+optional\"\n    },\n    \"exclusive\": {\n      \"type\": \"boolean\",\n  \
  \    \"title\": \"Exclusive when true, the server will ensure that this is the sole consumer from this queue\\n+optional\"\n    },\n    \"noLocal\": {\n      \"type\": \"boolean\",\n      \"title\": \"NoLocal flag is not supported by RabbitMQ\\n+optional\"\n    },\n    \"noWait\": {\n      \"type\": \"boolean\",\n      \"title\": \"NowWait when true, do not wait for the server to confirm the request and immediately begin deliveries\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-consume-config-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPConsumeConfig
---
