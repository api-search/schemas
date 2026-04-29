---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisStreamEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisStreamEventSource
properties_list:
- description: ''
  name: consumerGroup
  type: string
- description: ''
  name: db
  type: integer
- description: ''
  name: filter
  type: object
- description: ''
  name: hostAddress
  type: string
- description: ''
  name: maxMsgCountPerRead
  type: integer
- description: ''
  name: metadata
  type: object
- description: ''
  name: password
  type: object
- description: Streams to look for entries. XREADGROUP is used on all streams using a single consumer group.
  name: streams
  type: array
- description: ''
  name: tls
  type: object
- description: ''
  name: username
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-stream-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-stream-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-stream-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-stream-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisStreamEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisStreamEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"consumerGroup\": {\n      \"type\": \"string\",\n      \"title\": \"ConsumerGroup refers to the Redis stream consumer group that will be\\ncreated on all redis streams. Messages are read through this group. Defaults to 'argo-events-cg'\\n+optional\"\n    },\n    \"db\": {\n      \"type\": \"integer\",\n      \"title\": \"DB to use. If not specified, default DB 0 will be used.\\n+optional\"\n    },\n    \"filter\"\
  : {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"hostAddress\": {\n      \"type\": \"string\",\n      \"title\": \"HostAddress refers to the address of the Redis host/server (master instance)\"\n    },\n    \"maxMsgCountPerRead\": {\n      \"type\": \"integer\",\n      \"title\": \"MaxMsgCountPerRead holds the maximum number of messages per stream that will be read in each XREADGROUP of all streams\\nExample: if there are 2 streams and MaxMsgCountPerRead=10, then each XREADGROUP may read upto a total of 20 messages.\\nSame as COUNT option in XREADGROUP(https://redis.io/topics/streams-intro). Defaults to 10\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n\
  \    },\n    \"password\": {\n      \"title\": \"Password required for authentication if any.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"streams\": {\n      \"description\": \"Streams to look for entries. XREADGROUP is used on all streams using a single consumer group.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the redis client.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"title\": \"Username required for ACL style authentication if any.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-stream-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisStreamEventSource
---
