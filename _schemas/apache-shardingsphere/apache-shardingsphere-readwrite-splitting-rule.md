---
description: Read-write splitting configuration
layout: schema
name: ReadwriteSplittingRule
properties_list:
- description: Rule name
  name: name
  type: string
- description: Primary/write data source
  name: writeDataSourceName
  type: string
- description: Replica/read data sources
  name: readDataSourceNames
  type: array
- description: Load balancer algorithm name
  name: loadBalancerName
  type: string
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-readwrite-splitting-rule-schema.json
slug: apache-shardingsphere-readwrite-splitting-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-readwrite-splitting-rule-schema.json\",\n  \"title\": \"ReadwriteSplittingRule\",\n  \"description\": \"Read-write splitting configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Rule name\"\n    },\n    \"writeDataSourceName\": {\n      \"type\": \"string\",\n      \"description\": \"Primary/write data source\"\n    },\n    \"readDataSourceNames\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Replica/read data sources\"\n    },\n    \"loadBalancerName\": {\n      \"type\": \"string\",\n      \"description\": \"Load balancer algorithm name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-readwrite-splitting-rule-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: ReadwriteSplittingRule
---
