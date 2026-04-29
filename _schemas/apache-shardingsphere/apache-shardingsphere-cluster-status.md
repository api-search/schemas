---
description: ShardingSphere cluster status
layout: schema
name: ClusterStatus
properties_list:
- description: Deployment mode
  name: mode
  type: string
- description: ''
  name: instances
  type: array
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-cluster-status-schema.json
slug: apache-shardingsphere-cluster-status
source_filename: apache-shardingsphere-cluster-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-cluster-status-schema.json\",\n  \"title\": \"ClusterStatus\",\n  \"description\": \"ShardingSphere cluster status\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Standalone\",\n        \"Cluster\"\n      ],\n      \"description\": \"Deployment mode\"\n    },\n    \"instances\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Instance\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shardingsphere/refs/heads/main/json-schema/apache-shardingsphere-cluster-status-schema.json
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: ClusterStatus
---
