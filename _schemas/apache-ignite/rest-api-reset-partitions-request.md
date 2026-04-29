---
description: Reset partitions configuration.
layout: schema
name: ResetPartitionsRequest
properties_list:
- description: Name of the zone to reset partitions of. Without quotes, case-sensitive.
  name: zoneName
  type: string
- description: IDs of partitions to reset. All if empty.
  name: partitionIds
  type: array
- description: Fully-qualified name of the table to reset partitions of. Without quotes, case-sensitive.
  name: tableName
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-reset-partitions-request-schema.json
slug: rest-api-reset-partitions-request
source_filename: rest-api-reset-partitions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-reset-partitions-request-schema.json\",\n  \"title\": \"ResetPartitionsRequest\",\n  \"description\": \"Reset partitions configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"zoneName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the zone to reset partitions of. Without quotes, case-sensitive.\"\n    },\n    \"partitionIds\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of partitions to reset. All if empty.\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int32\"\n      }\n    },\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"Fully-qualified name of the table to reset partitions of. Without quotes, case-sensitive.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-reset-partitions-request-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: ResetPartitionsRequest
---
