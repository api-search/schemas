---
description: ''
layout: schema
name: LibertyServer
properties_list:
- description: Server name
  name: name
  type: string
- description: Liberty version
  name: wlpVersion
  type: string
- description: Product edition
  name: productEdition
  type: string
- description: Java version
  name: javaVersion
  type: string
- description: Java vendor
  name: javaVendor
  type: string
- description: ''
  name: serverStatus
  type: string
- description: Server uptime in milliseconds
  name: uptime
  type: integer
- description: Liberty installation directory
  name: installDirectory
  type: string
- description: Server configuration directory
  name: serverDirectory
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-admin-rest-liberty-server-schema.json
slug: websphere-liberty-admin-rest-liberty-server
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibertyServer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Server name\"\n    },\n    \"wlpVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Liberty version\"\n    },\n    \"productEdition\": {\n      \"type\": \"string\",\n      \"description\": \"Product edition\"\n    },\n    \"javaVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Java version\"\n    },\n    \"javaVendor\": {\n      \"type\": \"string\",\n      \"description\": \"Java vendor\"\n    },\n    \"serverStatus\": {\n      \"type\": \"string\"\n    },\n    \"uptime\": {\n      \"type\": \"integer\",\n      \"description\": \"Server uptime in milliseconds\"\n    },\n    \"installDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"Liberty installation directory\"\n    },\n    \"serverDirectory\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"Server configuration directory\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-admin-rest-liberty-server-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: LibertyServer
---
