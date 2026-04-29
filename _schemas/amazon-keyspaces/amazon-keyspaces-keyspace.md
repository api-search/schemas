---
description: An Amazon Keyspaces keyspace (Cassandra database).
layout: schema
name: Keyspace
properties_list:
- description: The name of the keyspace.
  name: keyspaceName
  type: string
- description: The Amazon Resource Name (ARN) of the keyspace.
  name: resourceArn
  type: string
- description: The replication strategy of the keyspace.
  name: replicationStrategy
  type: string
provider_name: Amazon Keyspaces
provider_slug: amazon-keyspaces
schema_file: json-schema/amazon-keyspaces-keyspace-schema.json
slug: amazon-keyspaces-keyspace
source_filename: amazon-keyspaces-keyspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-keyspaces/refs/heads/main/json-schema/amazon-keyspaces-keyspace-schema.json\",\n  \"title\": \"Keyspace\",\n  \"description\": \"An Amazon Keyspaces keyspace (Cassandra database).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyspaceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the keyspace.\",\n      \"example\": \"my_keyspace\"\n    },\n    \"resourceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the keyspace.\",\n      \"example\": \"arn:aws:cassandra:us-east-1:123456789012:/keyspace/my_keyspace\"\n    },\n    \"replicationStrategy\": {\n      \"type\": \"string\",\n      \"description\": \"The replication strategy of the keyspace.\",\n      \"example\": \"SINGLE_REGION\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-keyspaces/refs/heads/main/json-schema/amazon-keyspaces-keyspace-schema.json
tags:
- AWS
- Cassandra
- Database
- Managed Database
- NoSQL
- Wide Column
title: Keyspace
---
