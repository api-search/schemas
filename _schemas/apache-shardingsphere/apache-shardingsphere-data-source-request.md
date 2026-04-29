---
description: Request to add a data source
layout: schema
name: DataSourceRequest
properties_list:
- description: Data source name
  name: name
  type: string
- description: JDBC connection URL
  name: url
  type: string
- description: ''
  name: username
  type: string
- description: ''
  name: password
  type: string
- description: ''
  name: maxPoolSize
  type: integer
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-data-source-request-schema.json
slug: apache-shardingsphere-data-source-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-data-source-request-schema.json\",\n  \"title\": \"DataSourceRequest\",\n  \"description\": \"Request to add a data source\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Data source name\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"JDBC connection URL\"\n    },\n    \"username\": {\n      \"type\": \"string\"\n    },\n    \"password\": {\n      \"type\": \"string\"\n    },\n    \"maxPoolSize\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"url\",\n    \"username\",\n    \"password\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-data-source-request-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: DataSourceRequest
---
