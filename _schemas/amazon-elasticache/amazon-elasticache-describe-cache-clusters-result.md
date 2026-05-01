---
description: DescribeCacheClustersResult schema from Amazon ElastiCache API
layout: schema
name: DescribeCacheClustersResult
properties_list:
- description: ''
  name: CacheClusters
  type: array
- description: ''
  name: Marker
  type: string
provider_name: Amazon ElastiCache
provider_slug: amazon-elasticache
schema_file: json-schema/amazon-elasticache-describe-cache-clusters-result-schema.json
slug: amazon-elasticache-describe-cache-clusters-result
source_filename: amazon-elasticache-describe-cache-clusters-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elasticache/refs/heads/main/json-schema/amazon-elasticache-describe-cache-clusters-result-schema.json\",\n  \"title\": \"DescribeCacheClustersResult\",\n  \"description\": \"DescribeCacheClustersResult schema from Amazon ElastiCache API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CacheClusters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CacheCluster\"\n      }\n    },\n    \"Marker\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elasticache/refs/heads/main/json-schema/amazon-elasticache-describe-cache-clusters-result-schema.json
tags:
- Amazon Web Services
- Caching
- Database
- ElastiCache
- In-Memory
- Memcached
- Redis
title: DescribeCacheClustersResult
---
