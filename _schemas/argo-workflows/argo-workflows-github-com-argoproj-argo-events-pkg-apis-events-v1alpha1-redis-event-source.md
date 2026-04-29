---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisEventSource
properties_list:
- description: ''
  name: channels
  type: array
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
  name: jsonBody
  type: boolean
- description: ''
  name: metadata
  type: object
- description: ''
  name: namespace
  type: string
- description: ''
  name: password
  type: object
- description: ''
  name: tls
  type: object
- description: ''
  name: username
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"db\": {\n      \"type\": \"integer\",\n      \"title\": \"DB to use. If not specified, default DB 0 will be used.\\n+optional\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n\
  \    \"hostAddress\": {\n      \"type\": \"string\",\n      \"title\": \"HostAddress refers to the address of the Redis host/server\"\n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"JSONBody specifies that all event body payload coming from this\\nsource will be JSON\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"title\": \"Namespace to use to retrieve the password from. It should only be specified if password is declared\\n+optional\"\n    },\n    \"password\": {\n      \"title\": \"Password required for authentication if any.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration\
  \ for the redis client.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"title\": \"Username required for ACL style authentication if any.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisEventSource
---
