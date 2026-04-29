---
description: List of physical data sources
layout: schema
name: DataSourceList
properties_list:
- description: ''
  name: dataSources
  type: array
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-data-source-list-schema.json
slug: apache-shardingsphere-data-source-list
source_filename: apache-shardingsphere-data-source-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-data-source-list-schema.json\",\n  \"title\": \"DataSourceList\",\n  \"description\": \"List of physical data sources\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSources\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DataSource\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-data-source-list-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: DataSourceList
---
