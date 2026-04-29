---
description: Client schema from Apache EventMesh Admin API
layout: schema
name: Client
properties_list:
- description: ''
  name: env
  type: string
- description: ''
  name: idc
  type: string
- description: ''
  name: sys
  type: string
- description: ''
  name: ip
  type: string
- description: ''
  name: pid
  type: string
- description: ''
  name: protocol
  type: string
- description: ''
  name: group
  type: string
- description: ''
  name: topics
  type: array
provider_name: Apache EventMesh
provider_slug: apache-event-mesh
schema_file: json-schema/eventmesh-admin-client-schema.json
slug: eventmesh-admin-client
source_filename: eventmesh-admin-client-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/json-schema/eventmesh-admin-client-schema.json\",\n  \"title\": \"Client\",\n  \"description\": \"Client schema from Apache EventMesh Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"env\": {\n      \"type\": \"string\"\n    },\n    \"idc\": {\n      \"type\": \"string\"\n    },\n    \"sys\": {\n      \"type\": \"string\"\n    },\n    \"ip\": {\n      \"type\": \"string\"\n    },\n    \"pid\": {\n      \"type\": \"string\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HTTP\",\n        \"TCP\",\n        \"GRPC\"\n      ]\n    },\n    \"group\": {\n      \"type\": \"string\"\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/json-schema/eventmesh-admin-client-schema.json
tags:
- Apache
- CloudEvents
- Event-Driven
- Messaging
- Open Source
- Pub-Sub
- Serverless
title: Client
---
