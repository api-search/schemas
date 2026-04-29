---
description: Sharding configuration for a logical table
layout: schema
name: ShardingTable
properties_list:
- description: Logical table name
  name: logicTable
  type: string
- description: Actual data nodes expression (e.g. ds${0..1}.orders${0..3})
  name: actualDataNodes
  type: string
- description: ''
  name: databaseStrategy
  type: object
- description: ''
  name: tableStrategy
  type: object
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-sharding-table-schema.json
slug: apache-shardingsphere-sharding-table
source_filename: apache-shardingsphere-sharding-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-sharding-table-schema.json\",\n  \"title\": \"ShardingTable\",\n  \"description\": \"Sharding configuration for a logical table\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logicTable\": {\n      \"type\": \"string\",\n      \"description\": \"Logical table name\"\n    },\n    \"actualDataNodes\": {\n      \"type\": \"string\",\n      \"description\": \"Actual data nodes expression (e.g. ds${0..1}.orders${0..3})\"\n    },\n    \"databaseStrategy\": {\n      \"$ref\": \"#/components/schemas/ShardingStrategy\"\n    },\n    \"tableStrategy\": {\n      \"$ref\": \"#/components/schemas/ShardingStrategy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-sharding-table-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: ShardingTable
---
