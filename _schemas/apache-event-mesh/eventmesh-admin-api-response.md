---
description: ApiResponse schema from Apache EventMesh Admin API
layout: schema
name: ApiResponse
properties_list:
- description: Return code (0 for success)
  name: retCode
  type: integer
- description: Return message
  name: retMsg
  type: string
provider_name: Apache EventMesh
provider_slug: apache-event-mesh
schema_file: json-schema/eventmesh-admin-api-response-schema.json
slug: eventmesh-admin-api-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/json-schema/eventmesh-admin-api-response-schema.json\",\n  \"title\": \"ApiResponse\",\n  \"description\": \"ApiResponse schema from Apache EventMesh Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"retCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Return code (0 for success)\"\n    },\n    \"retMsg\": {\n      \"type\": \"string\",\n      \"description\": \"Return message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/json-schema/eventmesh-admin-api-response-schema.json
tags:
- Apache
- CloudEvents
- Event-Driven
- Messaging
- Open Source
- Pub-Sub
- Serverless
title: ApiResponse
---
