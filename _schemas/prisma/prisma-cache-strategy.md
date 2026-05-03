---
description: Cache configuration for Prisma Accelerate queries. Defines how query results should be cached using TTL (time-to-live) for fresh cache duration and SWR (stale-while-revalidate) for serving stale data while refreshing in the background. Tags enable targeted cache invalidation of specific query results.
layout: schema
name: Prisma Accelerate Cache Strategy
properties_list:
- description: Time-to-live in seconds. Cached results are served directly for this duration without querying the database. After TTL expires, the cache entry is considered stale.
  name: ttl
  type: integer
- description: Stale-while-revalidate time in seconds. After TTL expires, stale cached results are served to the client while a background refresh fetches fresh data from the database. The SWR window starts after TT
  name: swr
  type: integer
- description: Cache tags for targeted invalidation. Each tag is an alphanumeric string with underscores used to identify groups of cached queries that should be invalidated together.
  name: tags
  type: array
provider_name: Prisma
provider_slug: prisma
schema_file: json-schema/prisma-cache-strategy-schema.json
slug: prisma-cache-strategy
source_filename: prisma-cache-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://prisma.io/schemas/cache-strategy.json\",\n  \"title\": \"Prisma Accelerate Cache Strategy\",\n  \"description\": \"Cache configuration for Prisma Accelerate queries. Defines how query results should be cached using TTL (time-to-live) for fresh cache duration and SWR (stale-while-revalidate) for serving stale data while refreshing in the background. Tags enable targeted cache invalidation of specific query results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Time-to-live in seconds. Cached results are served directly for this duration without querying the database. After TTL expires, the cache entry is considered stale.\",\n      \"minimum\": 1,\n      \"examples\": [60, 300, 3600]\n    },\n    \"swr\": {\n      \"type\": \"integer\",\n      \"description\": \"Stale-while-revalidate time in seconds. After TTL expires,\
  \ stale cached results are served to the client while a background refresh fetches fresh data from the database. The SWR window starts after TTL expiration.\",\n      \"minimum\": 1,\n      \"examples\": [60, 300, 3600]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Cache tags for targeted invalidation. Each tag is an alphanumeric string with underscores used to identify groups of cached queries that should be invalidated together.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[a-zA-Z0-9_]{1,64}$\",\n        \"description\": \"A cache tag identifier (alphanumeric with underscores, max 64 characters)\"\n      },\n      \"maxItems\": 5,\n      \"uniqueItems\": true,\n      \"examples\": [[\"user_list\", \"active_users\"]]\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/json-schema/prisma-cache-strategy-schema.json
tags: []
title: Prisma Accelerate Cache Strategy
---
