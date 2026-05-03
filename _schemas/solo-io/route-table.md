---
description: A route table that provides modular and delegated routing configuration across teams and namespaces in Gloo Gateway.
layout: schema
name: Solo.io Gloo Gateway Route Table
properties_list:
- description: Resource metadata including name, namespace, and labels.
  name: metadata
  type: object
- description: Current status of the route table resource.
  name: status
  type: object
- description: List of routes defined in this route table.
  name: routes
  type: array
- description: Weight for route table ordering.
  name: weight
  type: integer
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/route-table.json
slug: route-table
source_filename: route-table.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/route-table.json\",\n  \"title\": \"Solo.io Gloo Gateway Route Table\",\n  \"description\": \"A route table that provides modular and delegated routing configuration across teams and namespaces in Gloo Gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"$ref\": \"resource-metadata.json\",\n      \"description\": \"Resource metadata including name, namespace, and labels.\"\n    },\n    \"status\": {\n      \"$ref\": \"resource-status.json\",\n      \"description\": \"Current status of the route table resource.\"\n    },\n    \"routes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"route.json\"\n      },\n      \"description\": \"List of routes defined in this route table.\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"Weight for route\
  \ table ordering.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/route-table.json
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
title: Solo.io Gloo Gateway Route Table
---
