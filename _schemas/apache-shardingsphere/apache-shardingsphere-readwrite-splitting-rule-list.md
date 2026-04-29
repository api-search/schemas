---
description: List of read-write splitting rules
layout: schema
name: ReadwriteSplittingRuleList
properties_list:
- description: ''
  name: rules
  type: array
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-readwrite-splitting-rule-list-schema.json
slug: apache-shardingsphere-readwrite-splitting-rule-list
source_filename: apache-shardingsphere-readwrite-splitting-rule-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-readwrite-splitting-rule-list-schema.json\",\n  \"title\": \"ReadwriteSplittingRuleList\",\n  \"description\": \"List of read-write splitting rules\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ReadwriteSplittingRule\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-readwrite-splitting-rule-list-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: ReadwriteSplittingRuleList
---
