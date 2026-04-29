---
description: Node info.
layout: schema
name: NodeInfo
properties_list:
- description: Unique node name.
  name: name
  type: string
- description: Node JDBC port.
  name: jdbcPort
  type: integer
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-node-info-schema.json
slug: rest-api-node-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-node-info-schema.json\",\n  \"title\": \"NodeInfo\",\n  \"description\": \"Node info.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique node name.\"\n    },\n    \"jdbcPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Node JDBC port.\",\n      \"format\": \"int32\"\n    }\n  },\n  \"required\": [\n    \"jdbcPort\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-node-info-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: NodeInfo
---
