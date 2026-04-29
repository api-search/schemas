---
description: Caching configuration for a resolver
layout: schema
name: CachingConfig
properties_list:
- description: TTL in seconds
  name: ttl
  type: integer
- description: Keys to use for caching
  name: cachingKeys
  type: array
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-caching-config-schema.json
slug: appsync-caching-config
source_filename: appsync-caching-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-caching-config-schema.json\",\n  \"title\": \"CachingConfig\",\n  \"description\": \"Caching configuration for a resolver\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"TTL in seconds\"\n    },\n    \"cachingKeys\": {\n      \"type\": \"array\",\n      \"description\": \"Keys to use for caching\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-caching-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: CachingConfig
---
