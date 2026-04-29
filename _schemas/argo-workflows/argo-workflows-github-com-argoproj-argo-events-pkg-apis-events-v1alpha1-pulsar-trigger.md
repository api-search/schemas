---
description: PulsarTrigger refers to the specification of the Pulsar trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PulsarTrigger
properties_list:
- description: ''
  name: authAthenzParams
  type: object
- description: ''
  name: authAthenzSecret
  type: object
- description: ''
  name: authTokenSecret
  type: object
- description: ''
  name: connectionBackoff
  type: object
- description: Parameters is the list of parameters that is applied to resolved Kafka trigger object.
  name: parameters
  type: array
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: ''
  name: tls
  type: object
- description: ''
  name: tlsAllowInsecureConnection
  type: boolean
- description: ''
  name: tlsTrustCertsSecret
  type: object
- description: ''
  name: tlsValidateHostname
  type: boolean
- description: ''
  name: topic
  type: string
- description: ''
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pulsar-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pulsar-trigger
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pulsar-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pulsar-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PulsarTrigger\",\n  \"description\": \"PulsarTrigger refers to the specification of the Pulsar trigger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authAthenzParams\": {\n      \"type\": \"object\",\n      \"title\": \"Authentication athenz parameters for the pulsar client.\\nRefer https://github.com/apache/pulsar-client-go/blob/master/pulsar/auth/athenz.go\\nEither token or athenz can be set to use auth.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"authAthenzSecret\": {\n      \"title\": \"Authentication athenz privateKey secret for the pulsar client.\\nAuthAthenzSecret\
  \ must be set if AuthAthenzParams is used.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"authTokenSecret\": {\n      \"title\": \"Authentication token for the pulsar client.\\nEither token or athenz can be set to use auth.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"connectionBackoff\": {\n      \"title\": \"Backoff holds parameters applied to connection.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff\"\n    },\n    \"parameters\": {\n      \"description\": \"Parameters is the list of parameters that is applied to resolved Kafka trigger object.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"payload\": {\n      \"description\": \"Payload is the list of key-value extracted from\
  \ an event payload to construct the request payload.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the pulsar client.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"tlsAllowInsecureConnection\": {\n      \"type\": \"boolean\",\n      \"title\": \"Whether the Pulsar client accept untrusted TLS certificate from broker.\\n+optional\"\n    },\n    \"tlsTrustCertsSecret\": {\n      \"title\": \"Trusted TLS certificate secret.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"tlsValidateHostname\": {\n      \"type\": \"boolean\",\n      \"title\": \"Whether the Pulsar client verify the validity of the host name from broker.\\n+optional\"\n    },\n    \"topic\": {\n    \
  \  \"type\": \"string\",\n      \"title\": \"Name of the topic.\\nSee https://pulsar.apache.org/docs/en/concepts-messaging/\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"title\": \"Configure the service URL for the Pulsar service.\\n+required\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pulsar-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PulsarTrigger
---
