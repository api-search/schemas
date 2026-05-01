---
description: Represents a kdb database within a FinSpace kdb environment.
layout: schema
name: KxDatabase
properties_list:
- description: ''
  name: databaseName
  type: string
- description: ''
  name: databaseArn
  type: string
- description: ''
  name: environmentId
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: createdTimestamp
  type: string
- description: ''
  name: lastModifiedTimestamp
  type: string
provider_name: Amazon FinSpace
provider_slug: amazon-finspace
schema_file: json-schema/amazon-finspace-kx-database-schema.json
slug: amazon-finspace-kx-database
source_filename: amazon-finspace-kx-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/json-schema/amazon-finspace-kx-database-schema.json\",\n  \"title\": \"KxDatabase\",\n  \"description\": \"Represents a kdb database within a FinSpace kdb environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"databaseName\": {\n      \"type\": \"string\"\n    },\n    \"databaseArn\": {\n      \"type\": \"string\"\n    },\n    \"environmentId\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"createdTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastModifiedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"databaseName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/json-schema/amazon-finspace-kx-database-schema.json
tags:
- Capital Markets
- Data Analytics
- Data Management
- Financial Services
title: KxDatabase
---
