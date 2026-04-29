---
description: List of ShardingSphere logical databases
layout: schema
name: DatabaseList
properties_list:
- description: ''
  name: databases
  type: array
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-database-list-schema.json
slug: apache-shardingsphere-database-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-database-list-schema.json\",\n  \"title\": \"DatabaseList\",\n  \"description\": \"List of ShardingSphere logical databases\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"databases\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Database\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-database-list-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: DatabaseList
---
