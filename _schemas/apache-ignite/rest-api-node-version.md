---
description: Node version.
layout: schema
name: NodeVersion
properties_list:
- description: Node version.
  name: version
  type: string
- description: Node product.
  name: product
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-node-version-schema.json
slug: rest-api-node-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-node-version-schema.json\",\n  \"title\": \"NodeVersion\",\n  \"description\": \"Node version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Node version.\"\n    },\n    \"product\": {\n      \"type\": \"string\",\n      \"description\": \"Node product.\"\n    }\n  },\n  \"required\": [\n    \"product\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-node-version-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: NodeVersion
---
