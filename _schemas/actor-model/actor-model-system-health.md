---
description: Overall health status of the actor system
layout: schema
name: SystemHealth
properties_list:
- description: Overall health
  name: status
  type: string
- description: Total active actors
  name: activeActors
  type: integer
- description: Current message throughput
  name: messagesPerSecond
  type: number
- description: Error rate (messages failed / total)
  name: errorRate
  type: number
- description: Messages sent to dead letter queue
  name: deadLetters
  type: integer
- description: Number of cluster nodes
  name: clusterSize
  type: integer
- description: System uptime in seconds
  name: uptime
  type: integer
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-system-health-schema.json
slug: actor-model-system-health
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-systemhealth-schema.json\",\n  \"title\": \"SystemHealth\",\n  \"description\": \"Overall health status of the actor system\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"healthy\",\n        \"degraded\",\n        \"unhealthy\"\n      ],\n      \"description\": \"Overall health\",\n      \"example\": \"healthy\"\n    },\n    \"activeActors\": {\n      \"type\": \"integer\",\n      \"description\": \"Total active actors\",\n      \"example\": 5000\n    },\n    \"messagesPerSecond\": {\n      \"type\": \"number\",\n      \"description\": \"Current message throughput\",\n      \"example\": 12500.5\n    },\n    \"errorRate\": {\n      \"type\": \"number\",\n      \"description\": \"Error rate (messages failed / total)\",\n      \"example\": 0.0001\n    },\n    \"deadLetters\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Messages sent to dead letter queue\",\n      \"example\": 3\n    },\n    \"clusterSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of cluster nodes\",\n      \"example\": 5\n    },\n    \"uptime\": {\n      \"type\": \"integer\",\n      \"description\": \"System uptime in seconds\",\n      \"example\": 86400\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-system-health-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: SystemHealth
---
