---
description: ShardingSphere Proxy instance
layout: schema
name: Instance
properties_list:
- description: Instance identifier
  name: instanceId
  type: string
- description: Instance status
  name: status
  type: string
- description: Host address
  name: host
  type: string
- description: Port number
  name: port
  type: integer
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-instance-schema.json
slug: apache-shardingsphere-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-instance-schema.json\",\n  \"title\": \"Instance\",\n  \"description\": \"ShardingSphere Proxy instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"Instance identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OK\",\n        \"CIRCUIT_BREAKER\"\n      ],\n      \"description\": \"Instance status\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Host address\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-instance-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: Instance
---
