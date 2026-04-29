---
description: ''
layout: schema
name: ControllerInfo
properties_list:
- description: Controller server name
  name: name
  type: string
- description: Controller hostname
  name: hostName
  type: string
- description: HTTPS port
  name: httpsPort
  type: integer
- description: Liberty version
  name: version
  type: string
- description: Total number of collective members
  name: memberCount
  type: integer
- description: Total number of clusters
  name: clusterCount
  type: integer
- description: Total number of hosts
  name: hostCount
  type: integer
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-collective-controller-rest-controller-info-schema.json
slug: websphere-liberty-collective-controller-rest-controller-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ControllerInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Controller server name\"\n    },\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"Controller hostname\"\n    },\n    \"httpsPort\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTPS port\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Liberty version\"\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of collective members\"\n    },\n    \"clusterCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of clusters\"\n    },\n    \"hostCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of hosts\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-collective-controller-rest-controller-info-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: ControllerInfo
---
