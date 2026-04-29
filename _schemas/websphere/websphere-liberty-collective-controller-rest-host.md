---
description: ''
layout: schema
name: Host
properties_list:
- description: Hostname
  name: name
  type: string
- description: Operating system
  name: os
  type: string
- description: Architecture
  name: arch
  type: string
- description: Number of processors
  name: processors
  type: integer
- description: Members on this host
  name: members
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-collective-controller-rest-host-schema.json
slug: websphere-liberty-collective-controller-rest-host
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Host\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system\"\n    },\n    \"arch\": {\n      \"type\": \"string\",\n      \"description\": \"Architecture\"\n    },\n    \"processors\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of processors\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"Members on this host\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-collective-controller-rest-host-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Host
---
