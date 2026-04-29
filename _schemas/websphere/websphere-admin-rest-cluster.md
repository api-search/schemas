---
description: ''
layout: schema
name: Cluster
properties_list:
- description: Cluster name
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: members
  type: array
- description: Whether to prefer local routing
  name: preferLocal
  type: boolean
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-admin-rest-cluster-schema.json
slug: websphere-admin-rest-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Cluster\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster name\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"members\": {\n      \"type\": \"array\"\n    },\n    \"preferLocal\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to prefer local routing\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-admin-rest-cluster-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Cluster
---
