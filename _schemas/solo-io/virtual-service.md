---
description: A virtual service that defines routing rules, security policies, and traffic management settings for incoming requests to Gloo Gateway.
layout: schema
name: Solo.io Gloo Gateway Virtual Service
properties_list:
- description: Resource metadata including name, namespace, and labels.
  name: metadata
  type: object
- description: Current status of the virtual service resource.
  name: status
  type: object
- description: Human-readable name for the virtual service.
  name: displayName
  type: string
- description: List of domains that this virtual service handles.
  name: domains
  type: array
- description: Ordered list of routing rules.
  name: routes
  type: array
- description: TLS/SSL configuration for the virtual service.
  name: sslConfig
  type: object
- description: Virtual host configuration including options.
  name: virtualHost
  type: object
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/virtual-service.json
slug: virtual-service
source_filename: virtual-service.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/virtual-service.json\",\n  \"title\": \"Solo.io Gloo Gateway Virtual Service\",\n  \"description\": \"A virtual service that defines routing rules, security policies, and traffic management settings for incoming requests to Gloo Gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"$ref\": \"resource-metadata.json\",\n      \"description\": \"Resource metadata including name, namespace, and labels.\"\n    },\n    \"status\": {\n      \"$ref\": \"resource-status.json\",\n      \"description\": \"Current status of the virtual service resource.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the virtual service.\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"\
  description\": \"List of domains that this virtual service handles.\"\n    },\n    \"routes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"route.json\"\n      },\n      \"description\": \"Ordered list of routing rules.\"\n    },\n    \"sslConfig\": {\n      \"type\": \"object\",\n      \"description\": \"TLS/SSL configuration for the virtual service.\"\n    },\n    \"virtualHost\": {\n      \"type\": \"object\",\n      \"description\": \"Virtual host configuration including options.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/virtual-service.json
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
title: Solo.io Gloo Gateway Virtual Service
---
