---
description: Sharding strategy definition
layout: schema
name: ShardingStrategy
properties_list:
- description: Strategy type
  name: type
  type: string
- description: Column used for sharding
  name: shardingColumn
  type: string
- description: Sharding algorithm reference
  name: shardingAlgorithmName
  type: string
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-sharding-strategy-schema.json
slug: apache-shardingsphere-sharding-strategy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-sharding-strategy-schema.json\",\n  \"title\": \"ShardingStrategy\",\n  \"description\": \"Sharding strategy definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"standard\",\n        \"complex\",\n        \"hint\",\n        \"none\"\n      ],\n      \"description\": \"Strategy type\"\n    },\n    \"shardingColumn\": {\n      \"type\": \"string\",\n      \"description\": \"Column used for sharding\"\n    },\n    \"shardingAlgorithmName\": {\n      \"type\": \"string\",\n      \"description\": \"Sharding algorithm reference\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-sharding-strategy-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: ShardingStrategy
---
