---
description: ''
layout: schema
name: EventProcessor
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: mode
  type: string
- description: ''
  name: isStreaming
  type: boolean
- description: ''
  name: fullName
  type: string
- description: ''
  name: tokenStoreIdentifier
  type: string
- description: ''
  name: activeThreads
  type: integer
- description: ''
  name: canPause
  type: boolean
- description: ''
  name: isRunning
  type: boolean
- description: ''
  name: isError
  type: boolean
provider_name: Axon Framework
provider_slug: axon-framework
schema_file: json-schema/axon-eventprocessor-schema.json
slug: axon-eventprocessor
source_filename: axon-eventprocessor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventProcessor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"mode\": {\n      \"type\": \"string\"\n    },\n    \"isStreaming\": {\n      \"type\": \"boolean\"\n    },\n    \"fullName\": {\n      \"type\": \"string\"\n    },\n    \"tokenStoreIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"activeThreads\": {\n      \"type\": \"integer\"\n    },\n    \"canPause\": {\n      \"type\": \"boolean\"\n    },\n    \"isRunning\": {\n      \"type\": \"boolean\"\n    },\n    \"isError\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/json-schema/axon-eventprocessor-schema.json
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
title: EventProcessor
---
