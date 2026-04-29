---
description: ''
layout: schema
name: ClusterStatus
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: membersStarted
  type: integer
- description: ''
  name: membersTotal
  type: integer
- description: ''
  name: message
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-collective-controller-rest-cluster-status-schema.json
slug: websphere-liberty-collective-controller-rest-cluster-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"membersStarted\": {\n      \"type\": \"integer\"\n    },\n    \"membersTotal\": {\n      \"type\": \"integer\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-collective-controller-rest-cluster-status-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: ClusterStatus
---
