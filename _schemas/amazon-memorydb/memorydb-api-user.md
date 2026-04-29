---
description: Represents a MemoryDB user.
layout: schema
name: User
properties_list:
- description: The names of the Access Control Lists to which the user belongs.
  name: ACLNames
  type: array
- description: The Amazon Resource Name (ARN) of the user.
  name: ARN
  type: string
- description: The name of the user.
  name: Name
  type: string
- description: Indicates the user status.
  name: Status
  type: string
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
schema_file: json-schema/memorydb-api-user-schema.json
slug: memorydb-api-user
source_filename: memorydb-api-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"Represents a MemoryDB user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ACLNames\": {\n      \"description\": \"The names of the Access Control Lists to which the user belongs.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"ARN\": {\n      \"description\": \"The Amazon Resource Name (ARN) of the user.\",\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"description\": \"The name of the user.\",\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"description\": \"Indicates the user status.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-user-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: User
---
