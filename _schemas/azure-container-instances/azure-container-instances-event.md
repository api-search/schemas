---
description: A container group or container instance event.
layout: schema
name: Event
properties_list:
- description: The count of the event.
  name: count
  type: integer
- description: The date-time of the earliest logged event.
  name: firstTimestamp
  type: string
- description: The date-time of the latest logged event.
  name: lastTimestamp
  type: string
- description: The event message.
  name: message
  type: string
- description: The event name.
  name: name
  type: string
- description: The event type.
  name: type
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-event-schema.json
slug: azure-container-instances-event
source_filename: azure-container-instances-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-event-schema.json\",\n  \"title\": \"Event\",\n  \"description\": \"A container group or container instance event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"description\": \"The count of the event.\",\n      \"type\": \"integer\"\n    },\n    \"firstTimestamp\": {\n      \"description\": \"The date-time of the earliest logged event.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"lastTimestamp\": {\n      \"description\": \"The date-time of the latest logged event.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"The event message.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The event name.\",\n\
  \      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The event type.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-event-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: Event
---
