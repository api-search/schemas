---
description: Sharding rule for a logical table
layout: schema
name: ShardingRule
properties_list:
- description: Rule name
  name: name
  type: string
- description: ''
  name: tables
  type: array
- description: ''
  name: bindingTables
  type: array
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-sharding-rule-schema.json
slug: apache-shardingsphere-sharding-rule
source_filename: apache-shardingsphere-sharding-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-sharding-rule-schema.json\",\n  \"title\": \"ShardingRule\",\n  \"description\": \"Sharding rule for a logical table\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Rule name\"\n    },\n    \"tables\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ShardingTable\"\n      }\n    },\n    \"bindingTables\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-sharding-rule-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: ShardingRule
---
