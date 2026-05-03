---
description: Common metadata for Gloo Gateway resources, including Kubernetes-style name, namespace, labels, and annotations.
layout: schema
name: Solo.io Gloo Gateway Resource Metadata
properties_list:
- description: Name of the resource.
  name: name
  type: string
- description: Namespace of the resource.
  name: namespace
  type: string
- description: Cluster where the resource resides.
  name: cluster
  type: string
- description: Labels attached to the resource.
  name: labels
  type: object
- description: Annotations attached to the resource.
  name: annotations
  type: object
- description: Version identifier for optimistic concurrency.
  name: resourceVersion
  type: string
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/resource-metadata.json
slug: resource-metadata
source_filename: resource-metadata.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/resource-metadata.json\",\n  \"title\": \"Solo.io Gloo Gateway Resource Metadata\",\n  \"description\": \"Common metadata for Gloo Gateway resources, including Kubernetes-style name, namespace, labels, and annotations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the resource.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Namespace of the resource.\"\n    },\n    \"cluster\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster where the resource resides.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels attached to the resource.\"\n    },\n    \"annotations\": {\n      \"type\": \"\
  object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Annotations attached to the resource.\"\n    },\n    \"resourceVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version identifier for optimistic concurrency.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/resource-metadata.json
tags:
- AI Gateway
- Analytics
- Automation
- Gateways
- Management
- Monetization
- Observability
- Platform
- Resiliency
- Security
- Service Mesh
- Traffic Control
title: Solo.io Gloo Gateway Resource Metadata
---
