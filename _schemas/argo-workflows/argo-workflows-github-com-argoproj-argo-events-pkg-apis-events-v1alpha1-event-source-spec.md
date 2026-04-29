---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceSpec schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceSpec
properties_list:
- description: ''
  name: amqp
  type: object
- description: ''
  name: azureEventsHub
  type: object
- description: ''
  name: azureQueueStorage
  type: object
- description: ''
  name: azureServiceBus
  type: object
- description: ''
  name: bitbucket
  type: object
- description: ''
  name: bitbucketserver
  type: object
- description: ''
  name: calendar
  type: object
- description: ''
  name: emitter
  type: object
- description: ''
  name: eventBusName
  type: string
- description: ''
  name: file
  type: object
- description: ''
  name: generic
  type: object
- description: ''
  name: gerrit
  type: object
- description: ''
  name: github
  type: object
- description: ''
  name: gitlab
  type: object
- description: ''
  name: hdfs
  type: object
- description: ''
  name: kafka
  type: object
- description: ''
  name: minio
  type: object
- description: ''
  name: mns
  type: object
- description: ''
  name: mqtt
  type: object
- description: ''
  name: nats
  type: object
- description: ''
  name: nsq
  type: object
- description: ''
  name: pubSub
  type: object
- description: ''
  name: pulsar
  type: object
- description: ''
  name: redis
  type: object
- description: ''
  name: redisStream
  type: object
- description: ''
  name: replicas
  type: integer
- description: ''
  name: resource
  type: object
- description: ''
  name: service
  type: object
- description: ''
  name: sftp
  type: object
- description: ''
  name: slack
  type: object
- description: ''
  name: sns
  type: object
- description: ''
  name: sqs
  type: object
- description: ''
  name: storageGrid
  type: object
- description: ''
  name: stripe
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: webhook
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-source-spec-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-source-spec
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-source-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-source-spec-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceSpec\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceSpec schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amqp\": {\n      \"type\": \"object\",\n      \"title\": \"AMQP event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AMQPEventSource\"\n      }\n    },\n    \"azureEventsHub\": {\n      \"type\": \"object\",\n      \"title\": \"AzureEventsHub event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventsHubEventSource\"\
  \n      }\n    },\n    \"azureQueueStorage\": {\n      \"type\": \"object\",\n      \"title\": \"AzureQueueStorage event source\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureQueueStorageEventSource\"\n      }\n    },\n    \"azureServiceBus\": {\n      \"type\": \"object\",\n      \"title\": \"Azure Service Bus event source\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusEventSource\"\n      }\n    },\n    \"bitbucket\": {\n      \"type\": \"object\",\n      \"title\": \"Bitbucket event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketEventSource\"\n      }\n    },\n    \"bitbucketserver\": {\n      \"type\": \"object\",\n      \"title\": \"Bitbucket Server event sources\",\n      \"additionalProperties\": {\n\
  \        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.BitbucketServerEventSource\"\n      }\n    },\n    \"calendar\": {\n      \"type\": \"object\",\n      \"title\": \"Calendar event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CalendarEventSource\"\n      }\n    },\n    \"emitter\": {\n      \"type\": \"object\",\n      \"title\": \"Emitter event source\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EmitterEventSource\"\n      }\n    },\n    \"eventBusName\": {\n      \"type\": \"string\",\n      \"title\": \"EventBusName references to a EventBus name. By default the value is \\\"default\\\"\"\n    },\n    \"file\": {\n      \"type\": \"object\",\n      \"title\": \"File event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.FileEventSource\"\
  \n      }\n    },\n    \"generic\": {\n      \"type\": \"object\",\n      \"title\": \"Generic event source\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GenericEventSource\"\n      }\n    },\n    \"gerrit\": {\n      \"type\": \"object\",\n      \"title\": \"Gerrit event source\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GerritEventSource\"\n      }\n    },\n    \"github\": {\n      \"type\": \"object\",\n      \"title\": \"Github event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GithubEventSource\"\n      }\n    },\n    \"gitlab\": {\n      \"type\": \"object\",\n      \"title\": \"Gitlab event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitlabEventSource\"\
  \n      }\n    },\n    \"hdfs\": {\n      \"type\": \"object\",\n      \"title\": \"HDFS event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HDFSEventSource\"\n      }\n    },\n    \"kafka\": {\n      \"type\": \"object\",\n      \"title\": \"Kafka event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaEventSource\"\n      }\n    },\n    \"minio\": {\n      \"type\": \"object\",\n      \"title\": \"Minio event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.S3Artifact\"\n      }\n    },\n    \"mns\": {\n      \"type\": \"object\",\n      \"title\": \"MNS event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.MNSEventSource\"\n\
  \      }\n    },\n    \"mqtt\": {\n      \"type\": \"object\",\n      \"title\": \"MQTT event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.MQTTEventSource\"\n      }\n    },\n    \"nats\": {\n      \"type\": \"object\",\n      \"title\": \"NATS event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSEventsSource\"\n      }\n    },\n    \"nsq\": {\n      \"type\": \"object\",\n      \"title\": \"NSQ event source\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NSQEventSource\"\n      }\n    },\n    \"pubSub\": {\n      \"type\": \"object\",\n      \"title\": \"PubSub event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PubSubEventSource\"\
  \n      }\n    },\n    \"pulsar\": {\n      \"type\": \"object\",\n      \"title\": \"Pulsar event source\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PulsarEventSource\"\n      }\n    },\n    \"redis\": {\n      \"type\": \"object\",\n      \"title\": \"Redis event source\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisEventSource\"\n      }\n    },\n    \"redisStream\": {\n      \"type\": \"object\",\n      \"title\": \"Redis stream source\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisStreamEventSource\"\n      }\n    },\n    \"replicas\": {\n      \"type\": \"integer\",\n      \"title\": \"Replicas is the event source deployment replicas\"\n    },\n    \"resource\": {\n      \"type\": \"object\",\n      \"title\": \"Resource event\
  \ sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ResourceEventSource\"\n      }\n    },\n    \"service\": {\n      \"title\": \"Service is the specifications of the service to expose the event source\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Service\"\n    },\n    \"sftp\": {\n      \"type\": \"object\",\n      \"title\": \"SFTP event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SFTPEventSource\"\n      }\n    },\n    \"slack\": {\n      \"type\": \"object\",\n      \"title\": \"Slack event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SlackEventSource\"\n      }\n    },\n    \"sns\": {\n      \"type\": \"object\",\n      \"title\": \"SNS event sources\"\
  ,\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SNSEventSource\"\n      }\n    },\n    \"sqs\": {\n      \"type\": \"object\",\n      \"title\": \"SQS event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SQSEventSource\"\n      }\n    },\n    \"storageGrid\": {\n      \"type\": \"object\",\n      \"title\": \"StorageGrid event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StorageGridEventSource\"\n      }\n    },\n    \"stripe\": {\n      \"type\": \"object\",\n      \"title\": \"Stripe event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StripeEventSource\"\n      }\n    },\n    \"template\": {\n      \"title\": \"Template is the pod specification\
  \ for the event source\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Template\"\n    },\n    \"webhook\": {\n      \"type\": \"object\",\n      \"title\": \"Webhook event sources\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookEventSource\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-source-spec-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceSpec
---
