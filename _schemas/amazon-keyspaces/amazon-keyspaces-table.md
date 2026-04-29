---
description: An Amazon Keyspaces table.
layout: schema
name: Table
properties_list:
- description: The name of the keyspace that the table is associated with.
  name: keyspaceName
  type: string
- description: The name of the table.
  name: tableName
  type: string
- description: The Amazon Resource Name (ARN) of the table.
  name: resourceArn
  type: string
- description: The current status of the table.
  name: status
  type: string
- description: The timestamp of when the table was created.
  name: creationTimestamp
  type: string
provider_name: Amazon Keyspaces
provider_slug: amazon-keyspaces
schema_file: json-schema/amazon-keyspaces-table-schema.json
slug: amazon-keyspaces-table
source_filename: amazon-keyspaces-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-keyspaces/refs/heads/main/json-schema/amazon-keyspaces-table-schema.json\",\n  \"title\": \"Table\",\n  \"description\": \"An Amazon Keyspaces table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyspaceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the keyspace that the table is associated with.\",\n      \"example\": \"my_keyspace\"\n    },\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table.\",\n      \"example\": \"my_table\"\n    },\n    \"resourceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the table.\",\n      \"example\": \"arn:aws:cassandra:us-east-1:123456789012:/keyspace/my_keyspace/table/my_table\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current\
  \ status of the table.\",\n      \"example\": \"ACTIVE\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"CREATING\",\n        \"UPDATING\",\n        \"DELETING\",\n        \"DELETED\",\n        \"RESTORING\",\n        \"INACCESSIBLE_ENCRYPTION_CREDENTIALS\"\n      ]\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp of when the table was created.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-keyspaces/refs/heads/main/json-schema/amazon-keyspaces-table-schema.json
tags:
- AWS
- Cassandra
- Database
- Managed Database
- NoSQL
- Wide Column
title: Table
---
