---
description: Node metadata information.
layout: schema
name: NodeMetadata
properties_list:
- description: The host exposed to REST API.
  name: restHost
  type: string
- description: The HTTP port exposed to REST API.
  name: httpPort
  type: integer
- description: The HTTPS port exposed to REST API.
  name: httpsPort
  type: integer
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-node-metadata-schema.json
slug: rest-api-node-metadata
source_filename: rest-api-node-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-node-metadata-schema.json\",\n  \"title\": \"NodeMetadata\",\n  \"description\": \"Node metadata information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"restHost\": {\n      \"type\": \"string\",\n      \"description\": \"The host exposed to REST API.\"\n    },\n    \"httpPort\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP port exposed to REST API.\",\n      \"format\": \"int32\"\n    },\n    \"httpsPort\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTPS port exposed to REST API.\",\n      \"format\": \"int32\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-node-metadata-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: NodeMetadata
---
