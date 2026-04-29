---
description: A Node represents a Kubernetes node within a cluster managed by CAST AI, including its instance type, state, and labels.
layout: schema
name: CAST AI Node
properties_list:
- description: Unique identifier for the node.
  name: id
  type: string
- description: Name of the node.
  name: name
  type: string
- description: Cloud provider instance type of the node.
  name: instanceType
  type: string
- description: Current state of the node.
  name: state
  type: string
- description: Timestamp when the node was created.
  name: createdAt
  type: string
- description: Key-value labels assigned to the node.
  name: labels
  type: object
provider_name: CAST AI
provider_slug: cast-ai
schema_file: json-schema/node.json
slug: node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cast-ai/blob/main/json-schema/node.json\",\n  \"title\": \"CAST AI Node\",\n  \"description\": \"A Node represents a Kubernetes node within a cluster managed by CAST AI, including its instance type, state, and labels.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the node.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the node.\"\n    },\n    \"instanceType\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider instance type of the node.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ready\",\n        \"not_ready\",\n        \"draining\",\n        \"deleting\"\n      ],\n      \"description\": \"Current state of the node.\"\n    },\n  \
  \  \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the node was created.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value labels assigned to the node.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/json-schema/node.json
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
title: CAST AI Node
---
