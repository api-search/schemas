---
description: An Access Control List.
layout: schema
name: ACL
properties_list:
- description: The Amazon Resource Name (ARN) of the ACL.
  name: ARN
  type: string
- description: The name of the Access Control List.
  name: Name
  type: string
- description: Indicates the current status of the ACL.
  name: Status
  type: string
- description: The list of user names that belong to the ACL.
  name: UserNames
  type: array
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
schema_file: json-schema/memorydb-api-acl-schema.json
slug: memorydb-api-acl
source_filename: memorydb-api-acl-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-acl-schema.json\",\n  \"title\": \"ACL\",\n  \"description\": \"An Access Control List.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ARN\": {\n      \"description\": \"The Amazon Resource Name (ARN) of the ACL.\",\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"description\": \"The name of the Access Control List.\",\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"description\": \"Indicates the current status of the ACL.\",\n      \"type\": \"string\"\n    },\n    \"UserNames\": {\n      \"description\": \"The list of user names that belong to the ACL.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-acl-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ACL
---
