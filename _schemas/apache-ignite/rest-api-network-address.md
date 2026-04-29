---
description: Node network address information.
layout: schema
name: NetworkAddress
properties_list:
- description: Name of the host node runs on.
  name: host
  type: string
- description: Port the node runs on.
  name: port
  type: integer
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-network-address-schema.json
slug: rest-api-network-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-network-address-schema.json\",\n  \"title\": \"NetworkAddress\",\n  \"description\": \"Node network address information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the host node runs on.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port the node runs on.\",\n      \"format\": \"int32\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-network-address-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: NetworkAddress
---
