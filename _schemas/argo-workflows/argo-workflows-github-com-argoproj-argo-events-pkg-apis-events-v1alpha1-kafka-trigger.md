---
description: KafkaTrigger refers to the specification of the Kafka trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaTrigger
properties_list:
- description: ''
  name: compress
  type: boolean
- description: ''
  name: flushFrequency
  type: integer
- description: ''
  name: headers
  type: object
- description: Parameters is the list of parameters that is applied to resolved Kafka trigger object.
  name: parameters
  type: array
- description: ''
  name: partition
  type: integer
- description: The partitioning key for the messages put on the Kafka topic. +optional.
  name: partitioningKey
  type: string
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: RequiredAcks used in producer to tell the broker how many replica acknowledgements Defaults to 1 (Only wait for the leader to ack). +optional.
  name: requiredAcks
  type: integer
- description: ''
  name: sasl
  type: object
- description: ''
  name: schemaRegistry
  type: object
- description: ''
  name: secureHeaders
  type: array
- description: ''
  name: tls
  type: object
- description: ''
  name: topic
  type: string
- description: URL of the Kafka broker, multiple URLs separated by comma.
  name: url
  type: string
- description: ''
  name: version
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-trigger
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaTrigger\",\n  \"description\": \"KafkaTrigger refers to the specification of the Kafka trigger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"compress\": {\n      \"type\": \"boolean\",\n      \"title\": \"Compress determines whether to compress message or not.\\nDefaults to false.\\nIf set to true, compresses message using snappy compression.\\n+optional\"\n    },\n    \"flushFrequency\": {\n      \"type\": \"integer\",\n      \"title\": \"FlushFrequency refers to the frequency in milliseconds to flush batches.\\nDefaults to 500 milliseconds.\\n+optional\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n  \
  \    \"title\": \"Headers for the Kafka Messages.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"parameters\": {\n      \"description\": \"Parameters is the list of parameters that is applied to resolved Kafka trigger object.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"partition\": {\n      \"type\": \"integer\",\n      \"title\": \"+optional\\nDEPRECATED\"\n    },\n    \"partitioningKey\": {\n      \"description\": \"The partitioning key for the messages put on the Kafka topic.\\n+optional.\",\n      \"type\": \"string\"\n    },\n    \"payload\": {\n      \"description\": \"Payload is the list of key-value extracted from an event payload to construct the request payload.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\
  \n      }\n    },\n    \"requiredAcks\": {\n      \"description\": \"RequiredAcks used in producer to tell the broker how many replica acknowledgements\\nDefaults to 1 (Only wait for the leader to ack).\\n+optional.\",\n      \"type\": \"integer\"\n    },\n    \"sasl\": {\n      \"title\": \"SASL configuration for the kafka client\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SASLConfig\"\n    },\n    \"schemaRegistry\": {\n      \"title\": \"Schema Registry configuration to producer message with avro format\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SchemaRegistryConfig\"\n    },\n    \"secureHeaders\": {\n      \"type\": \"array\",\n      \"title\": \"Secure Headers stored in Kubernetes Secrets for the Kafka messages.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SecureHeader\"\n     \
  \ }\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the Kafka producer.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"title\": \"Name of the topic.\\nMore info at https://kafka.apache.org/documentation/#intro_topics\"\n    },\n    \"url\": {\n      \"description\": \"URL of the Kafka broker, multiple URLs separated by comma.\",\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"title\": \"Specify what kafka version is being connected to enables certain features in sarama, defaults to 1.0.0\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaTrigger
---
