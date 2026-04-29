---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPEventSource
properties_list:
- description: ''
  name: auth
  type: object
- description: ''
  name: connectionBackoff
  type: object
- description: ''
  name: consume
  type: object
- description: ''
  name: exchangeDeclare
  type: object
- description: ''
  name: exchangeName
  type: string
- description: ''
  name: exchangeType
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
  name: queueBind
  type: object
- description: ''
  name: queueDeclare
  type: object
- description: ''
  name: routingKey
  type: string
- description: ''
  name: tls
  type: object
- description: ''
  name: url
  type: string
- description: ''
  name: urlSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"auth\": {\n      \"title\": \"Auth hosts secret selectors for username and password\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BasicAuth\"\n    },\n    \"connectionBackoff\": {\n      \"title\": \"Backoff holds parameters applied to connection.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff\"\n    },\n   \
  \ \"consume\": {\n      \"title\": \"Consume holds the configuration to immediately starts delivering queued messages\\nFor more information, visit https://pkg.go.dev/github.com/rabbitmq/amqp091-go#Channel.Consume\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPConsumeConfig\"\n    },\n    \"exchangeDeclare\": {\n      \"title\": \"ExchangeDeclare holds the configuration for the exchange on the server\\nFor more information, visit https://pkg.go.dev/github.com/rabbitmq/amqp091-go#Channel.ExchangeDeclare\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPExchangeDeclareConfig\"\n    },\n    \"exchangeName\": {\n      \"type\": \"string\",\n      \"title\": \"ExchangeName is the exchange name\\nFor more information, visit https://www.rabbitmq.com/tutorials/amqp-concepts.html\"\n    },\n    \"exchangeType\": {\n      \"type\": \"string\",\n      \"title\": \"ExchangeType\
  \ is rabbitmq exchange type\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"JSONBody specifies that all event body payload coming from this\\nsource will be JSON\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"queueBind\": {\n      \"title\": \"QueueBind holds the configuration that binds an exchange to a queue so that publishings to the\\nexchange will be routed to the queue when the publishing routing key matches the binding routing key\\nFor more information, visit https://pkg.go.dev/github.com/rabbitmq/amqp091-go#Channel.QueueBind\\n+optional\",\n\
  \      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPQueueBindConfig\"\n    },\n    \"queueDeclare\": {\n      \"title\": \"QueueDeclare holds the configuration of a queue to hold messages and deliver to consumers.\\nDeclaring creates a queue if it doesn't already exist, or ensures that an existing queue matches\\nthe same parameters\\nFor more information, visit https://pkg.go.dev/github.com/rabbitmq/amqp091-go#Channel.QueueDeclare\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPQueueDeclareConfig\"\n    },\n    \"routingKey\": {\n      \"type\": \"string\",\n      \"title\": \"Routing key for bindings\"\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the amqp client.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"title\": \"URL for rabbitmq\
  \ service\"\n    },\n    \"urlSecret\": {\n      \"title\": \"URLSecret is secret reference for rabbitmq service URL\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-amqp-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPEventSource
---
