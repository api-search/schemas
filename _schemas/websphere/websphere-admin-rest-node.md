---
description: ''
layout: schema
name: Node
properties_list:
- description: Node name
  name: name
  type: string
- description: Hostname of the node
  name: hostName
  type: string
- description: Operating system platform
  name: platformOS
  type: string
- description: ''
  name: servers
  type: array
- description: Whether the node configuration is synchronized
  name: synchronized
  type: boolean
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-admin-rest-node-schema.json
slug: websphere-admin-rest-node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Node\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Node name\"\n    },\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the node\"\n    },\n    \"platformOS\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system platform\"\n    },\n    \"servers\": {\n      \"type\": \"array\"\n    },\n    \"synchronized\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the node configuration is synchronized\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-admin-rest-node-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Node
---
