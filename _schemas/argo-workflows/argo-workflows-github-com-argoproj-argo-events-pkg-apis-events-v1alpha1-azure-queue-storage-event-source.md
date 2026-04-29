---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureQueueStorageEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureQueueStorageEventSource
properties_list:
- description: ''
  name: connectionString
  type: object
- description: ''
  name: decodeMessage
  type: boolean
- description: ''
  name: dlq
  type: boolean
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
  name: queueName
  type: string
- description: ''
  name: storageAccountName
  type: string
- description: ''
  name: waitTimeInSeconds
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-queue-storage-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-queue-storage-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-queue-storage-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-queue-storage-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureQueueStorageEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureQueueStorageEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionString\": {\n      \"title\": \"ConnectionString is the connection string to access Azure Queue Storage. If this fields is not provided\\nit will try to access via Azure AD with StorageAccountName.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"decodeMessage\": {\n      \"type\": \"boolean\",\n      \"title\": \"DecodeMessage specifies\
  \ if all the messages should be base64 decoded.\\nIf set to true the decoding is done before the evaluation of JSONBody\\n+optional\"\n    },\n    \"dlq\": {\n      \"type\": \"boolean\",\n      \"title\": \"DLQ specifies if a dead-letter queue is configured for messages that can't be processed successfully.\\nIf set to true, messages with invalid payload won't be acknowledged to allow to forward them farther to the dead-letter queue.\\nThe default value is false.\\n+optional\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"JSONBody specifies that all event body payload coming from this\\nsource will be JSON\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\\
  n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"queueName\": {\n      \"type\": \"string\",\n      \"title\": \"QueueName is the name of the queue\"\n    },\n    \"storageAccountName\": {\n      \"type\": \"string\",\n      \"title\": \"StorageAccountName is the name of the storage account where the queue is. This field is necessary to\\naccess via Azure AD (managed identity) and it is ignored if ConnectionString is set.\\n+optional\"\n    },\n    \"waitTimeInSeconds\": {\n      \"type\": \"integer\",\n      \"title\": \"WaitTimeInSeconds is the duration (in seconds) for which the event source waits between empty results from the queue.\\nThe default value is 3 seconds.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-queue-storage-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureQueueStorageEventSource
---
