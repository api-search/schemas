---
description: Represents the output of a CreateParameterGroup operation.
layout: schema
name: ParameterGroup
properties_list:
- description: The Amazon Resource Name (ARN) of the parameter group.
  name: ARN
  type: string
- description: A description of the parameter group.
  name: Description
  type: string
- description: The name of the parameter group family.
  name: Family
  type: string
- description: The name of the parameter group.
  name: Name
  type: string
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
schema_file: json-schema/memorydb-api-parameter-group-schema.json
slug: memorydb-api-parameter-group
source_filename: memorydb-api-parameter-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-parameter-group-schema.json\",\n  \"title\": \"ParameterGroup\",\n  \"description\": \"Represents the output of a CreateParameterGroup operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ARN\": {\n      \"description\": \"The Amazon Resource Name (ARN) of the parameter group.\",\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"description\": \"A description of the parameter group.\",\n      \"type\": \"string\"\n    },\n    \"Family\": {\n      \"description\": \"The name of the parameter group family.\",\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"description\": \"The name of the parameter group.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-parameter-group-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ParameterGroup
---
