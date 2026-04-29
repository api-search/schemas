---
description: Standard Kubernetes object metadata
layout: schema
name: ObjectMeta
properties_list:
- description: Name of the resource, unique within a namespace
  name: name
  type: string
- description: Kubernetes namespace the resource belongs to
  name: namespace
  type: string
- description: Key-value pairs for organizing and selecting resources
  name: labels
  type: object
- description: Key-value pairs for storing arbitrary non-identifying metadata
  name: annotations
  type: object
- description: Timestamp when the resource was created
  name: creationTimestamp
  type: string
- description: Sequence number representing a specific generation of the resource
  name: generation
  type: integer
- description: Opaque value for optimistic concurrency control
  name: resourceVersion
  type: string
- description: Unique identifier for the resource
  name: uid
  type: string
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-object-meta-schema.json
slug: ambassador-object-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectMeta\",\n  \"type\": \"object\",\n  \"description\": \"Standard Kubernetes object metadata\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the resource, unique within a namespace\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes namespace the resource belongs to\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs for organizing and selecting resources\"\n    },\n    \"annotations\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs for storing arbitrary non-identifying metadata\"\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the resource was created\"\n    },\n    \"generation\": {\n      \"type\": \"integer\",\n      \"description\": \"Sequence number\
  \ representing a specific generation of the resource\"\n    },\n    \"resourceVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Opaque value for optimistic concurrency control\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the resource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-object-meta-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: ObjectMeta
---
