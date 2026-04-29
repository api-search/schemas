---
description: ''
layout: schema
name: SBQueue
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Service Bus
provider_slug: azure-service-bus
schema_file: json-schema/azure-service-bus-sb-queue-schema.json
slug: azure-service-bus-sb-queue
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SBQueue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-service-bus/refs/heads/main/json-schema/azure-service-bus-sb-queue-schema.json
tags:
- Azure
- Cloud
- Enterprise
- Message Broker
- Messaging
- Pub/Sub
- Queues
title: SBQueue
---
