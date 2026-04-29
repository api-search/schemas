---
description: Physical data source configuration
layout: schema
name: DataSource
properties_list:
- description: Data source name
  name: name
  type: string
- description: JDBC connection URL
  name: url
  type: string
- description: Database username
  name: username
  type: string
- description: Maximum connection pool size
  name: maxPoolSize
  type: integer
- description: Minimum connection pool size
  name: minPoolSize
  type: integer
- description: Connection pool type (HikariCP, etc.)
  name: type
  type: string
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-data-source-schema.json
slug: apache-shardingsphere-data-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-data-source-schema.json\",\n  \"title\": \"DataSource\",\n  \"description\": \"Physical data source configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Data source name\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"JDBC connection URL\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Database username\"\n    },\n    \"maxPoolSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum connection pool size\"\n    },\n    \"minPoolSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum connection pool size\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Connection\
  \ pool type (HikariCP, etc.)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-data-source-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: DataSource
---
