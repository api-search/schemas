---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaEventSource
properties_list:
- description: 'Yaml format Sarama config for Kafka connection. It follows the struct of sarama.Config. See https://github.com/IBM/sarama/blob/main/config.go e.g. consumer: fetch: min: 1 net: MaxOpenRequests: 5 +opti'
  name: config
  type: string
- description: Backoff holds parameters applied to connection.
  name: connectionBackoff
  type: object
- description: ''
  name: consumerGroup
  type: object
- description: ''
  name: filter
  type: object
- description: ''
  name: jsonBody
  type: boolean
- description: ''
  name: limitEventsPerSecond
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: partition
  type: string
- description: ''
  name: sasl
  type: object
- description: ''
  name: schemaRegistry
  type: object
- description: ''
  name: tls
  type: object
- description: ''
  name: topic
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: version
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"config\": {\n      \"description\": \"Yaml format Sarama config for Kafka connection.\\nIt follows the struct of sarama.Config. See https://github.com/IBM/sarama/blob/main/config.go\\ne.g.\\n\\nconsumer:\\n  fetch:\\n    min: 1\\nnet:\\n  MaxOpenRequests: 5\\n\\n+optional\",\n      \"type\": \"string\"\n    },\n    \"connectionBackoff\": {\n      \"description\": \"Backoff holds parameters applied to connection.\",\n      \"$ref\"\
  : \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff\"\n    },\n    \"consumerGroup\": {\n      \"title\": \"Consumer group for kafka client\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaConsumerGroup\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"JSONBody specifies that all event body payload coming from this\\nsource will be JSON\\n+optional\"\n    },\n    \"limitEventsPerSecond\": {\n      \"type\": \"string\",\n      \"title\": \"Sets a limit on how many events get read from kafka per second.\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n\
  \      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"partition\": {\n      \"type\": \"string\",\n      \"title\": \"Partition name\\n+optional\"\n    },\n    \"sasl\": {\n      \"title\": \"SASL configuration for the kafka client\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SASLConfig\"\n    },\n    \"schemaRegistry\": {\n      \"title\": \"Schema Registry configuration for consumer message with Avro format\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SchemaRegistryConfig\"\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the kafka client.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"title\": \"Topic name\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"title\": \"URL\
  \ to kafka cluster, multiple URLs separated by comma\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"title\": \"Specify what kafka version is being connected to enables certain features in sarama, defaults to 1.0.0\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaEventSource
---
