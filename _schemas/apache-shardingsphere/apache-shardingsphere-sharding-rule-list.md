---
description: List of sharding rules
layout: schema
name: ShardingRuleList
properties_list:
- description: ''
  name: rules
  type: array
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-sharding-rule-list-schema.json
slug: apache-shardingsphere-sharding-rule-list
source_filename: apache-shardingsphere-sharding-rule-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-sharding-rule-list-schema.json\",\n  \"title\": \"ShardingRuleList\",\n  \"description\": \"List of sharding rules\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ShardingRule\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-sharding-rule-list-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: ShardingRuleList
---
